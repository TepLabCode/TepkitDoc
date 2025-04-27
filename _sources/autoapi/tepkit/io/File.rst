tepkit.io.File
==============

.. py:class:: tepkit.io.File


   The base class for all files.



Attributes
----------

.. csv-table::
   :header: "Attribute", "Default Value", "Description"

   "``default_dir_path``", "``'./'``", "The default path of located directory of file when use ``from_dir()`` ."
   "``default_file_name``", "``None``", "The default name of file when use ``from_dir()`` ."
   "``source_path``", "``None``", "Record the path of the file when use ``from_file()`` or ``from_dir()`` ."






Methods
-------

.. autoapisummary::

   tepkit.io.File.from_file
   tepkit.io.File.from_dir
   tepkit.io.File.to_file




All Members
-----------


.. py:attribute:: default_dir_path
   :no-index:
   :type:  PathLike
   :value: './'


   The default path of located directory of file when use ``from_dir()`` .



.. py:attribute:: default_file_name
   :no-index:
   :type:  str
   :value: None


   The default name of file when use ``from_dir()`` .



.. py:attribute:: source_path
   :no-index:
   :type:  pathlib.Path | None
   :value: None


   Record the path of the file when use ``from_file()`` or ``from_dir()`` .



.. py:method:: from_file(path: tepkit.utils.typing_tools.PathLike) -> Self
   :no-index:
   :classmethod:


   Read a file by its ``path`` .

   >>> file1 = File.from_file("example.txt")
   >>> file2 = File.from_file("../example.txt")



.. py:method:: from_dir(path: tepkit.utils.typing_tools.PathLike = None, file_name: str = None) -> Self
   :no-index:
   :classmethod:


   Read a file named ``cls.default_file_name`` in the ``cls.default_dir_path``.

   >>> file1 = File.from_dir()

   You can also specify the dirctory path or the file name:

   >>> file2 = File.from_dir("./result")
   >>> file3 = File.from_dir(file_name = "file_name.txt")
   >>> file4 = File.from_dir("./result", file_name = "file_name.txt")



.. py:method:: to_file(path: tepkit.utils.typing_tools.PathLike)
   :no-index:
   :classmethod:
   :abstractmethod:


   Write the data of the object to a file.





# File Manipulation / System I.O Notes

This topic is important to me because I think its cool that I can modify my computer files by using code.

## [Retrospective 3](https://connerkt.github.io/Reading-Notes/401/Class03/Retro03)

## References

[File and Stream I/0](https://docs.microsoft.com/en-us/dotnet/standard/io/index)

[Write to a file](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file)

[Read to a file](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)

## File and Stream I/O Notes

This refers to the transfer of data either to or from a storage medium.

The **System.IO** namespaces contain types that enable reading and writing.

You can use these types to interact with files and directories.

Here are some of the key takeaways of the library:

### The .NET Standard IO library provides classes and APIs for working with input and output operations in .NET applications.

- The library is part of the .NET Standard, which is a set of APIs that are available across different .NET implementations.
- The primary namespace for IO operations is **System.IO**.
- **System.IO** contains classes and methods for working with files, directories, streams, and other input/output operations.
- The **File** class provides static methods for working with files, such as reading from or writing to files, creating or deleting files, and getting file information.
- The **Directory** class provides static methods for working with directories, including creating, deleting, and enumerating directories.
- The **Path** class provides methods for working with file and directory paths, such as combining paths, getting file extensions, and manipulating paths.
- The **FileStream** class enables reading from or writing to a file as a stream of bytes.
- The **StreamReader** and **StreamWriter** classes provide higher-level functionality for reading and writing text to files, using specific encodings.
- The **MemoryStream** class represents a stream that uses a block of memory as its backing store.
- The **BinaryReader** and **BinaryWriter** classes enable reading from and writing to streams in binary format.
- The **Stream** class is an abstract base class that provides a generic view of a sequence of bytes. Many other stream classes derive from **Stream**.
- The **StreamReader** and **StreamWriter** classes are commonly used for reading and writing text data from/to files.
- The **StreamReader** reads characters from a byte stream in a specific encoding and converts them into characters.
- The **StreamWriter** writes characters to a byte stream in a specific encoding.
- The **File** class provides methods for working with files, such as reading, writing, copying, deleting, and moving files.
- The **FileInfo** class provides instance methods and properties for working with individual files, such as getting file attributes and dates, and creating or deleting files.
- The **Directory** class provides methods for working with directories, such as creating, deleting, moving, and enumerating directories.
- The **DirectoryInfo** class provides instance methods and properties for working with directories, such as getting directory attributes and dates, and creating or deleting directories.
- The **Path** class provides methods for manipulating file and directory paths, such as combining paths, getting file extensions, or extracting file names.
- The **Path** class also provides methods for checking the validity of paths, resolving relative paths, and working with UNC paths.
- The **Path** class includes platform-specific members for working with paths on Windows, Unix, or macOS systems.
- The **DriveInfo** class provides information about drives on the system, such as available space, drive format, and drive type.
- The **DriveInfo** class also provides methods for working with drives, such as formatting drives or retrieving drive volumes.
- The **FileSystemWatcher** class enables monitoring of file system events, such as changes to files or directories, creations or deletions of files, or renaming files.
- The **FileSystemWatcher** can raise events when specific file system changes occur.
- The **MemoryStream** class represents a stream that uses a block of memory as its backing store instead of a file.
- The **MemoryStream** can be used to read from or write to an in-memory buffer, without the need for physical files.
- The **BinaryReader** class enables reading primitive data types from a stream in binary format.
- The **BinaryWriter** class enables writing primitive data types to a stream in binary format.
- The **BinaryReader** and **BinaryWriter** classes provide methods for reading and writing values of different data types, such as integers, floats, strings, and more.

## How to write to a file

The following classes and methods are typically used to write text to a file:

StreamWriter contains methods to write to a file synchronously (Write and WriteLine) or asynchronously (WriteAsync and WriteLineAsync).

File provides static methods to write text to a file such as WriteAllLines and WriteAllText, or to append text to a file such as AppendAllLines, AppendAllText, and AppendText.

Path is for strings that have file or directory path information. It contains the Combine method and in .NET Core 2.1 and later, the Join and TryJoin methods. These methods let you concatenate strings for building a file or directory path.

## How to read a file

The System.IO.BinaryWriter and System.IO.BinaryReader classes are used for writing and reading data other than character strings.

        using System;
        using System.IO;

        class MyStream
        {
            private const string FILE_NAME = "Test.data";

            public static void Main()
            {
                if (File.Exists(FILE_NAME))
                {
                    Console.WriteLine($"{FILE_NAME} already exists!");
                    return;
                }

                using (FileStream fs = new FileStream(FILE_NAME, FileMode.CreateNew))
                {
                    using (BinaryWriter w = new BinaryWriter(fs))
                    {
                        for (int i = 0; i < 11; i++)
                        {
                            w.Write(i);
                        }
                    }
                }

                using (FileStream fs = new FileStream(FILE_NAME, FileMode.Open, FileAccess.Read))
                {
                    using (BinaryReader r = new BinaryReader(fs))
                    {
                        for (int i = 0; i < 11; i++)
                        {
                            Console.WriteLine(r.ReadInt32());
                        }
                    }
                }
            }
        }


// The example creates a file named "Test.data" and writes the integers 0 through 10 to it in binary format.
// It then writes the contents of Test.data to the console with each integer on a separate line.

## Things I want to know more about

How to apply this in a bigger setting (Like using it to automate your file creation etc)
I want to learn how to use this for fun stuff(Deleting files if they match a certain criteria)

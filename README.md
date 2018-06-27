## copypath

This is a Windows Explorer shell extension that will allow you to right click on a drive or file system object and copy the path of the file to the clipbpoard. If the drive is a mapped drive or the file system object exits on a mapped drive it will resolve the full UNC path.

**Project Description**  
This extension is intended to make the task of finding and sharing the UNC path for a mapped drive easier as I often need to find this information from colleagues or pass this information to colleagues. I created this utility to make it simpler.  
  
This is a Windows Explorer shell extension that will allow you to right click on a drive or file system object and copy the path of the file to the clipbpoard. If the drive is a mapped drive or the file system object exits on a mapped drive it will resolve the full UNC path.  
  
  
**Supported Systems**  
Although designed for Windows XP, I will maintain builds of this extension for the following versions of Windows.

-   Windows 7
-   Windows Server 2008
-   Windows Vista
-   Windows XP
-   Windows 2003

  
  
**Installation**  
To install this extension follow these steps

1.  Download latest build for your operating system from this page
2.  Extract the DLL to a folder on your hard drive such as %WINDIR%\System32
3.  From the command prompt issue the following commands
    1.  cd %WINDIR%\System32
    2.  regsvr32 CopyPath.dll

  
The extension will now be installed so you can right click on a drive or file system object and you will see the option 'Copy Path'  
  
  
**Uninstall**  
To uninstall this extension follow these steps

1.  Open command prompt and issue the following commands.  _Note that I assume you placed the CopyPath.dll into the %WINDIR%\System32 directory_
    1.  cd %WINDIR%\System32
    2.  regsvr32 /U CopyPath.dll
    3.  del CopyPath.dll
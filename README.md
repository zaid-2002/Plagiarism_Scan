# Plagiarism Checker

This application is designed to detect plagiarism in Word (.docx), PDF (.pdf), and Text (.txt) files with three distinct modes: **One-to-One Mode**, **Multi-File Mode**, and **Cross-File Mode**.

## Modes Overview

- **One-to-One Mode:**

  ![image](https://github.com/user-attachments/assets/0cc1547d-5c3d-44d3-adbd-e4ad7961e79a)
  - This mode checks plagiarism between a source file and a target file. The result will be a copy of the source file, where any text found to be plagiarized from the target file will be highlighted.

- **Multi-File Mode:**

  ![image](https://github.com/user-attachments/assets/ce35701f-ba6e-474d-ba87-4890c406d862)
  - In this mode, the application checks multiple source files against multiple target files. For example, if the source files contain `File1.docx` and the target files contain `File2.docx` and `File3.docx`, the application will check `File1.docx` against both `File2.docx` and `File3.docx`. The results will be compiled into an Excel file, showing the percentage of plagiarism between `File1.docx` and each of the target files.
  - Result example

    ![image](https://github.com/user-attachments/assets/2c06bfba-452d-4a74-afd5-58b0d58b0613)

- **Cross-File Mode:**

  ![image](https://github.com/user-attachments/assets/7027f302-4b48-4935-980f-de3a1ced5cce)
  - This mode performs cross-checks among all selected files, generating an Excel report similar to the one produced in Multi-File Mode. Each file will be checked against the others, providing a comprehensive overview of potential plagiarism within the group of files.
  - Result example

    ![image](https://github.com/user-attachments/assets/5077d8c9-81e6-43dd-8146-8ac3db2bedb7)

This application is a powerful tool for ensuring originality in documents and preventing plagiarism across multiple file formats.

## Plagiarism Detection Level

The plagiarism detection level is a configurable setting within the application that determines the minimum sequence of consecutive words that must match between two files for the text to be flagged as potential plagiarism. 

For example, if the detection level is set to 4, then a sequence of at least 4 identical consecutive words must be present in both the source and target files for the text to be highlighted as plagiarized. This setting allows users to control the sensitivity of the plagiarism detection process. A lower level might result in more text being flagged as plagiarized, including common phrases, while a higher level ensures that only longer, potentially more significant matches are considered.

Adjusting the detection level helps balance between catching potential plagiarism and avoiding false positives, depending on the specific needs of the user or the nature of the documents being compared.


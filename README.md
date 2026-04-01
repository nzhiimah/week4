# week4 - Metadata Analysis Lab

1.  |Tool Used | File       |Link                |
    |----------|----------- |-----------------   |
    |exiftool  | ocean.jpg  |https://exif.tools/ |


**Steps Performed :**

1. opened the link provided
2. clicked the **Choose File** button
3. choose ocean.jpg from the provided ZIP file 
4. clicked the **Upload File** button
5. reviewed the file metadata

**Metadata Found**
- **File Type:** JPEG
- **File Name:** phpqRmOa5
- **MIME Type:** image/jpeg
- **Primary Platform:** Apple Computer Inc.
- **Comment:** THIS IS THE HIDDEN FLAG
- **Image Size:** 640x425

**Analysis** 

This metadata shows the internal properties of the image file.
From the output, we can identify:

- the file format is a valid JPEG image
- MIME type confirms it is an image file
- the **comment field contains the hidden flag** 
- information is useful in **digital forensics and file verification**

---

2.  |Tool Used | File          |Link                |
    |----------|-----------    |-----------------   |
    |Hexeditor | computer.jpg  |https://hexed.it/   |


**Steps Performed :**

1. opened the link provided
2. clicked the **Open File** button
3. choose computer.jpg from the provided ZIP file
4. reviewed the file information & data inspector

**Data Inspector Findings**
- **Offset:** 00000000
- **Hex Value:** FF D8 FF
- **UNIX 31-bit DateTime:** 2089-08-14 13:13:35 UTC
- **File Size:** 588,975 bytes (576 KiB) 

**Analysis** 

- The hex values show the raw binary content of the file.
- The file signature confirms that it is a valid JPEG image.
- The Data Inspector helps identify hidden text or suspicious data inside the file.
- This method is useful for **digital forensics and file verification.**

---

3.  |Tool Used | File          |Link                                   |
    |----------|-----------    |-----------------                      |
    |strings   | computer.jpg  | https://www.dcode.fr/strings-extractor|


**Steps Performed :**

1. go to the **STRINGS EXTRACTOR** section
2. clicked the **Choose File** button
3. choose computer.jpg from the provided ZIP file 
4. clicked the **EXTRACT** button
5. reviewed the results displayed on the left side

**Result Found**
- **Error** ! Sorry :( 
- **TEXT** : EMPTY/INVALID

<img width="455" height="169" alt="Screenshot 2026-04-01 150111" src="https://github.com/user-attachments/assets/7840febc-dcbb-4122-9771-b9ecd046005c" />

**Analysis** 

- No readable strings were successfully extracted from the file.
- The file may not contain embedded text data.
- The image could contain only binary image data without hidden readable content.
- This result helps confirm that no obvious text-based evidence is present.


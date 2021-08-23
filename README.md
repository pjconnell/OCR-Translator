**What does this do?**

This is a program that uses open source Optical Character Recognition (OCR) to convert a PDF to text (.txt), which is then translated into English.

**How does it work?**

The OCR portion of this program utilizes pytesseract (more information at: https://pypi.org/project/pytesseract/). The translation is completed using Google Translate's Python API (more information at: https://pypi.org/project/googletrans/).

**How do I use it?**

First, it's important to note that this program was built to work on Google Drive (it was developed as part of a collaborative research project that required extensive translation of foreign academic papers). The colab notebook will look for the "input PDF" - i.e., document you want translated - on Google Drive and it will generate and save an English translation .txt file to Google Drive. Accordingly, the most important initial steps are to get the appropriate folders set up in Google drive so that the notebook can access / generate the files that it needs.

The following steps will walk you through that set-up process.

*Step 1* - Open the Google Colab notebook and save it to your Google Drive. I suggest putting it in a folder titled "Foreign Text OCR", or something similar, so you can keep the input/output files all in one place.

*Step 2* - Create two new folders in the same file where you saved the Colab notebook. one should be titled "Input PDFs" and the other "Output TXTs".

*Step 3* - Save the .xlsx file "Language Key" as a google sheet in the same folder. When you are done, the folder should look like this:

![alt text](https://github.com/pjconnell/OCR-Translator/blob/main/file_setup.png)

*Step 4* - Next, save the PDF file(s) you want to translate in the "Input PDFs" folder.

*Step 5* - You're ready to go! Open the Colab notebook and follow the prompts for running the OCR + Translation program.

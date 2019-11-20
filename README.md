# Word Canary Checker

This is a small script that checks for canary tokens hidden in Microsoft Word files. It cannot stop the canary from calling home if you open the file, it just notifies you if it is in the file.

## Why

The idea was to scan for canary tokens embedded in pdfs. But those tokens only activate automatically if you open the pdf with Adobe Reader. If you use Adobe Acrobat DC then you will be notified and able to block the canary. Canary pdfs generated from canarytokens.org are suspicously blank anyway. Someone who uses MS Word for whatever reason in this day and age is still vulnerable to this exploit, however.

## Use

Only works on unix distros (macOS or Linux).

If you do not have `unzip` then you will need to install that.

Place it in the same folder as the file you need too scan and then

```bash
chmod +x canary_check.sh
./canary_check.sh
```

and give it the name of the Word doc.





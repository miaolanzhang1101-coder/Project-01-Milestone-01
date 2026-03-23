Data Exploration and Findings
After generating a metadata CSV from my Google Drive export, I explored the dataset to identify patterns, surprises, and potential risks. The dataset contains a mix of file types, with DOCX files dominating (72 files), followed by PDFs (16), XLSX (3), ZIPs (2), PNGs (2), and single instances of MOV, MP4, HTML, and DS_Store files. This distribution suggests that the export primarily consists of textual documents, likely personal or work-related files, with only a small fraction of multimedia content.
# file_type
docx        72
pdf         16
xlsx         3
zip          2
png          2
DS_Store     1
mov          1
html         1
mp4          1
Name: count, dtype: int64

The timestamp analysis shows that the earliest and latest files are essentially identical, both on March 23, 2026, which indicates that the export was created as a snapshot of my data at a single moment rather than accumulated over time. 

# Earliest and latest files
Earliest file: 2026-03-23 17:41:40.237266064
Latest file: 2026-03-23 17:41:41.173211575

Searching for potentially sensitive filenames using keywords like “password,” “key,” or “token” returned no matches, suggesting that, based on filenames alone, the export does not contain obvious security risks. However, this does not guarantee that sensitive information is absent, as passwords or confidential data could be embedded within PDFs, DOCXs, or spreadsheets.

#scary files
Empty DataFrame
Columns: [file_name, file_type, file_size_kb, created_time, modified_time, folder_path]
Index: []


In conclusion, this exploration of my Google Drive export reveals both the strengths and limitations of personal metadata. While the dataset accurately reflects the types and quantities of files I store, it provides only a static snapshot, missing historical trends and the full content of documents. The predominance of DOCX and PDF files aligns with expectations, and the lack of obviously sensitive filenames suggests minimal immediate risk. However, the low representation of multimedia files and the uniform timestamps highlight gaps in the export, showing that Google Takeout captures structure more than lived activity.

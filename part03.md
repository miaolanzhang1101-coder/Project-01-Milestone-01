Findings:
The dataset contains 99 files with attributes including file type, size, and timestamps.

1. File type distribution is highly uneven
Certain file types (such as PDFs and media files like MP4/MOV) account for a disproportionately large share of total storage, even though they may not be the most frequent file types.
2. Storage is dominated by large media files
While smaller file types (e.g., .xlsx, .html, .DS_Store) appear frequently, they contribute very little to total storage usage. In contrast, a small number of large files significantly impact overall storage consumption.
3. File system has long-tail behavior
There is a classic “long tail” distribution:
many small files with minimal impact
a few very large files that dominate system resources



Other findings:
Larger files tend to appear sporadically rather than consistently, suggesting that storage spikes are event-driven (e.g., uploads, exports, or media additions).
File creation is not uniform over time, but rather clustered, indicating bursts of activity rather than steady usage.
File types are not evenly distributed across time, which may reflect different usage phases (e.g., early-stage documents vs. later-stage media or exports)

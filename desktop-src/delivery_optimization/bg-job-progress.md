---
title: BG\_JOB\_PROGRESS structure
description: The BG\_JOB\_PROGRESS structure provides job-related progress information, such as the number of bytes and files transferred. For upload jobs, the progress applies to the upload file, not the reply file.
ms.assetid: 'F07BBDDE-FD34-4779-9E17-3789A8098616'
keywords: ["BG_JOB_PROGRESS structure"]
topic_type:
- apiref
api_name:
- BG_JOB_PROGRESS
api_location:
- deliveryoptimization.h
api_type:
- HeaderDef
---

# BG\_JOB\_PROGRESS structure

The **BG\_JOB\_PROGRESS** structure provides job-related progress information, such as the number of bytes and files transferred. For upload jobs, the progress applies to the upload file, not the reply file.

## Syntax


```C++
typedef struct _BG_JOB_PROGRESS {
  UINT64 BytesTotal;
  UINT64 BytesTransferred;
  ULONG �FilesTotal;
  ULONG �FilesTransferred;
} BG_JOB_PROGRESS;
```



## Members

<dl> <dt>

**BytesTotal**
</dt> <dd>

Total number of bytes to transfer for all files in the job. If the value is BG\_SIZE\_UNKNOWN, the total size of all files in the job has not been determined. DO does not set this value if it cannot determine the size of one of the files. For example, if the specified file or server does not exist, DO cannot determine the size of the file.

If you are downloading ranges from the file, **BytesTotal** includes the total number of bytes you want to download from the file.

</dd> <dt>

**BytesTransferred**
</dt> <dd>

Number of bytes transferred.

</dd> <dt>

**FilesTotal**
</dt> <dd>

Total number of files to transfer for this job.

</dd> <dt>

**FilesTransferred**
</dt> <dd>

Number of files transferred.

</dd> </dl>

## Requirements



|                                     |                                                                                                   |
|-------------------------------------|---------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�10, version 1709 \[desktop apps only\]<br/>                                         |
| Minimum supported server<br/> | Windows Server, version 1709 \[desktop apps only\]<br/>                                     |
| Header<br/>                   | <dl> <dt>Deliveryoptimization.h</dt> </dl> |



## See also

<dl> <dt>

[**BG\_FILE\_PROGRESS**](bg-file-progress.md)
</dt> <dt>

[**IBackgroundCopyJob::GetProgress**](ibackgroundcopyjob-getprogress.md)
</dt> </dl>

�

�





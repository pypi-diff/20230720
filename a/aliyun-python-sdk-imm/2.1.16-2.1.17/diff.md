# Comparing `tmp/aliyun-python-sdk-imm-2.1.16.tar.gz` & `tmp/aliyun-python-sdk-imm-2.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-imm-2.1.16.tar", last modified: Wed Jul  5 05:50:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-imm-2.1.17.tar", last modified: Thu Jul 20 08:55:08 2023, max compression
```

## Comparing `aliyun-python-sdk-imm-2.1.16.tar` & `aliyun-python-sdk-imm-2.1.17.tar`

### file list

```diff
@@ -1,117 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/
--rw-r--r--   0 root         (0) root         (0)      575 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6134 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/
--rw-r--r--   0 root         (0) root         (0)     2643 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1654 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1885 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2070 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1903 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2695 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2396 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     3804 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2609 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2900 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     4105 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2872 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     4567 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2116 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py
--rw-r--r--   0 root         (0) root         (0)     4440 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetBindingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1873 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     2056 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListBatchesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListBindingsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListProjectsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3393 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListTriggersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4516 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2951 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     1608 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2128 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1907 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1843 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2023-07-05 05:50:10.000000 aliyun-python-sdk-imm-2.1.16/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6014 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/
+-rw-r--r--   0 root         (0) root         (0)     2643 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2070 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2872 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4567 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetBindingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListBatchesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListBindingsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1805 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListProjectsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3393 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListTriggersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-07-20 08:55:08.000000 aliyun-python-sdk-imm-2.1.17/setup.py
```

### Comparing `aliyun-python-sdk-imm-2.1.16/LICENSE` & `aliyun-python-sdk-imm-2.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/PKG-INFO` & `aliyun-python-sdk-imm-2.1.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imm
-Version: 2.1.16
+Version: 2.1.17
 Summary: The imm module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imm
```

### Comparing `aliyun-python-sdk-imm-2.1.16/README.rst` & `aliyun-python-sdk-imm-2.1.17/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/PKG-INFO` & `aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-imm
-Version: 2.1.16
+Version: 2.1.17
 Summary: The imm module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-imm
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyun_python_sdk_imm.egg-info/SOURCES.txt` & `aliyun-python-sdk-imm-2.1.17/aliyun_python_sdk_imm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py
 aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py
 aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py
 aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py
 aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py
 aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py
 aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py
-aliyunsdkimm/request/v20200930/GenerateVideoPlaylistRequest.py
 aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py
 aliyunsdkimm/request/v20200930/GetBatchRequest.py
 aliyunsdkimm/request/v20200930/GetBindingRequest.py
 aliyunsdkimm/request/v20200930/GetDatasetRequest.py
 aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py
 aliyunsdkimm/request/v20200930/GetFileMetaRequest.py
 aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py
@@ -82,15 +81,14 @@
 aliyunsdkimm/request/v20200930/ListBatchesRequest.py
 aliyunsdkimm/request/v20200930/ListBindingsRequest.py
 aliyunsdkimm/request/v20200930/ListDatasetsRequest.py
 aliyunsdkimm/request/v20200930/ListProjectsRequest.py
 aliyunsdkimm/request/v20200930/ListRegionsRequest.py
 aliyunsdkimm/request/v20200930/ListTasksRequest.py
 aliyunsdkimm/request/v20200930/ListTriggersRequest.py
-aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py
 aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py
 aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py
 aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py
 aliyunsdkimm/request/v20200930/QueryStoriesRequest.py
 aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py
 aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py
 aliyunsdkimm/request/v20200930/ResumeBatchRequest.py
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/endpoint.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AddImageMosaicRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AddStoryFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/AttachOSSBucketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchDeleteFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchGetFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchGetFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchIndexFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/BatchUpdateFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CompareImageFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateArchiveFileInspectionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateBindingRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateCompressPointCloudTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateCustomizedStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFacesSearchingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFigureClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFigureClustersMergingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFileCompressionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateFileUncompressionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageModerationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageSplicingTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateImageToPDFTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateLocationDateClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateMediaConvertTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateOfficeConversionTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateProjectRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateSimilarImageClusteringTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateStoryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateVideoLabelClassificationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/CreateVideoModerationTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteBindingRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,12 +42,7 @@
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_query_param('ProjectName', ProjectName)
 	def get_URI(self): # String
 		return self.get_query_params().get('URI')
 
 	def set_URI(self, URI):  # String
 		self.add_query_param('URI', URI)
-	def get_Cleanup(self): # Boolean
-		return self.get_query_params().get('Cleanup')
-
-	def set_Cleanup(self, Cleanup):  # Boolean
-		self.add_query_param('Cleanup', Cleanup)
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteLocationDateClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DeleteTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetachOSSBucketRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageBodiesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCarsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCodesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageCroppingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageLabelsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectImageScoreRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectMediaMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/DetectTextAnomalyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ExtractDocumentTextRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/FuzzyQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GenerateWebofficeTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetBindingRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetBindingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetImageModerationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetOSSBucketAttachmentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetProjectRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetStoryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetStoryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetTaskRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetVideoLabelClassificationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/GetVideoModerationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/IndexFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListBatchesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListBatchesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListBindingsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListBindingsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListDatasetsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListProjectsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListProjectsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListRegionsRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListTasksRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListTasksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ListTriggersRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ListTriggersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/LiveTranscodingRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,30 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkimm.endpoint import endpoint_data
 import json
 
-class LiveTranscodingRequest(RpcRequest):
+class SearchImageFigureClusterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'imm', '2020-09-30', 'LiveTranscoding','imm')
+		RpcRequest.__init__(self, 'imm', '2020-09-30', 'SearchImageFigureCluster','imm')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_DatasetName(self): # String
+		return self.get_query_params().get('DatasetName')
+
+	def set_DatasetName(self, DatasetName):  # String
+		self.add_query_param('DatasetName', DatasetName)
 	def get_ProjectName(self): # String
 		return self.get_query_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_query_param('ProjectName', ProjectName)
 	def get_CredentialConfig(self): # Struct
 		return self.get_query_params().get('CredentialConfig')
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryFigureClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryLocationDateClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QuerySimilarImageClustersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/QueryStoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/RefreshWebofficeTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/RemoveStoryFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ResumeBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/ResumeTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SearchImageFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,40 +15,44 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkimm.endpoint import endpoint_data
-import json
 
-class SearchImageFigureClusterRequest(RpcRequest):
+class SemanticQueryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'imm', '2020-09-30', 'SearchImageFigureCluster','imm')
+		RpcRequest.__init__(self, 'imm', '2020-09-30', 'SemanticQuery','imm')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_NextToken(self): # String
+		return self.get_query_params().get('NextToken')
+
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
 	def get_DatasetName(self): # String
 		return self.get_query_params().get('DatasetName')
 
 	def set_DatasetName(self, DatasetName):  # String
 		self.add_query_param('DatasetName', DatasetName)
 	def get_ProjectName(self): # String
 		return self.get_query_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_query_param('ProjectName', ProjectName)
-	def get_CredentialConfig(self): # Struct
-		return self.get_query_params().get('CredentialConfig')
+	def get_Query(self): # String
+		return self.get_query_params().get('Query')
 
-	def set_CredentialConfig(self, CredentialConfig):  # Struct
-		self.add_query_param("CredentialConfig", json.dumps(CredentialConfig))
-	def get_SourceURI(self): # String
-		return self.get_query_params().get('SourceURI')
+	def set_Query(self, Query):  # String
+		self.add_query_param('Query', Query)
+	def get_MaxResults(self): # Integer
+		return self.get_query_params().get('MaxResults')
 
-	def set_SourceURI(self, SourceURI):  # String
-		self.add_query_param('SourceURI', SourceURI)
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SemanticQueryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,44 +15,50 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkimm.endpoint import endpoint_data
+import json
 
-class SemanticQueryRequest(RpcRequest):
+class UpdateLocationDateClusterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'imm', '2020-09-30', 'SemanticQuery','imm')
+		RpcRequest.__init__(self, 'imm', '2020-09-30', 'UpdateLocationDateCluster','imm')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
+	def get_CustomLabels(self): # Map
+		return self.get_query_params().get('CustomLabels')
 
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
+	def set_CustomLabels(self, CustomLabels):  # Map
+		self.add_query_param("CustomLabels", json.dumps(CustomLabels))
+	def get_Title(self): # String
+		return self.get_query_params().get('Title')
+
+	def set_Title(self, Title):  # String
+		self.add_query_param('Title', Title)
 	def get_DatasetName(self): # String
 		return self.get_query_params().get('DatasetName')
 
 	def set_DatasetName(self, DatasetName):  # String
 		self.add_query_param('DatasetName', DatasetName)
 	def get_ProjectName(self): # String
 		return self.get_query_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_query_param('ProjectName', ProjectName)
-	def get_Query(self): # String
-		return self.get_query_params().get('Query')
+	def get_CustomId(self): # String
+		return self.get_query_params().get('CustomId')
 
-	def set_Query(self, Query):  # String
-		self.add_query_param('Query', Query)
-	def get_MaxResults(self): # Integer
-		return self.get_query_params().get('MaxResults')
+	def set_CustomId(self, CustomId):  # String
+		self.add_query_param('CustomId', CustomId)
+	def get_ObjectId(self): # String
+		return self.get_query_params().get('ObjectId')
 
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_query_param('MaxResults', MaxResults)
+	def set_ObjectId(self, ObjectId):  # String
+		self.add_query_param('ObjectId', ObjectId)
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SimpleQueryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SuspendBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/SuspendTriggerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateBatchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateDatasetRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateFigureClusterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateFileMetaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateLocationDateClusterRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,48 +17,53 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkimm.endpoint import endpoint_data
 import json
 
-class UpdateLocationDateClusterRequest(RpcRequest):
+class UpdateStoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'imm', '2020-09-30', 'UpdateLocationDateCluster','imm')
+		RpcRequest.__init__(self, 'imm', '2020-09-30', 'UpdateStory','imm')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_CustomLabels(self): # Map
-		return self.get_query_params().get('CustomLabels')
+	def get_CustomLabels(self): # String
+		return self.get_body_params().get('CustomLabels')
 
-	def set_CustomLabels(self, CustomLabels):  # Map
-		self.add_query_param("CustomLabels", json.dumps(CustomLabels))
-	def get_Title(self): # String
-		return self.get_query_params().get('Title')
+	def set_CustomLabels(self, CustomLabels):  # String
+		self.add_body_params('CustomLabels', CustomLabels)
+	def get_Cover(self): # Struct
+		return self.get_body_params().get('Cover')
 
-	def set_Title(self, Title):  # String
-		self.add_query_param('Title', Title)
+	def set_Cover(self, Cover):  # Struct
+		self.add_body_params("Cover", json.dumps(Cover))
 	def get_DatasetName(self): # String
-		return self.get_query_params().get('DatasetName')
+		return self.get_body_params().get('DatasetName')
 
 	def set_DatasetName(self, DatasetName):  # String
-		self.add_query_param('DatasetName', DatasetName)
+		self.add_body_params('DatasetName', DatasetName)
 	def get_ProjectName(self): # String
-		return self.get_query_params().get('ProjectName')
+		return self.get_body_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
-		self.add_query_param('ProjectName', ProjectName)
+		self.add_body_params('ProjectName', ProjectName)
 	def get_CustomId(self): # String
-		return self.get_query_params().get('CustomId')
+		return self.get_body_params().get('CustomId')
 
 	def set_CustomId(self, CustomId):  # String
-		self.add_query_param('CustomId', CustomId)
+		self.add_body_params('CustomId', CustomId)
 	def get_ObjectId(self): # String
-		return self.get_query_params().get('ObjectId')
+		return self.get_body_params().get('ObjectId')
 
 	def set_ObjectId(self, ObjectId):  # String
-		self.add_query_param('ObjectId', ObjectId)
+		self.add_body_params('ObjectId', ObjectId)
+	def get_StoryName(self): # String
+		return self.get_body_params().get('StoryName')
+
+	def set_StoryName(self, StoryName):  # String
+		self.add_body_params('StoryName', StoryName)
```

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateProjectRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-imm-2.1.16/aliyunsdkimm/request/v20200930/UpdateStoryRequest.py` & `aliyun-python-sdk-imm-2.1.17/aliyunsdkimm/request/v20200930/UpdateTriggerRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,53 +17,43 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkimm.endpoint import endpoint_data
 import json
 
-class UpdateStoryRequest(RpcRequest):
+class UpdateTriggerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'imm', '2020-09-30', 'UpdateStory','imm')
+		RpcRequest.__init__(self, 'imm', '2020-09-30', 'UpdateTrigger','imm')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_CustomLabels(self): # String
-		return self.get_body_params().get('CustomLabels')
+	def get_Id(self): # String
+		return self.get_body_params().get('Id')
 
-	def set_CustomLabels(self, CustomLabels):  # String
-		self.add_body_params('CustomLabels', CustomLabels)
-	def get_Cover(self): # Struct
-		return self.get_body_params().get('Cover')
-
-	def set_Cover(self, Cover):  # Struct
-		self.add_body_params("Cover", json.dumps(Cover))
-	def get_DatasetName(self): # String
-		return self.get_body_params().get('DatasetName')
-
-	def set_DatasetName(self, DatasetName):  # String
-		self.add_body_params('DatasetName', DatasetName)
+	def set_Id(self, Id):  # String
+		self.add_body_params('Id', Id)
 	def get_ProjectName(self): # String
 		return self.get_body_params().get('ProjectName')
 
 	def set_ProjectName(self, ProjectName):  # String
 		self.add_body_params('ProjectName', ProjectName)
-	def get_CustomId(self): # String
-		return self.get_body_params().get('CustomId')
+	def get_Tags(self): # Map
+		return self.get_body_params().get('Tags')
 
-	def set_CustomId(self, CustomId):  # String
-		self.add_body_params('CustomId', CustomId)
-	def get_ObjectId(self): # String
-		return self.get_body_params().get('ObjectId')
-
-	def set_ObjectId(self, ObjectId):  # String
-		self.add_body_params('ObjectId', ObjectId)
-	def get_StoryName(self): # String
-		return self.get_body_params().get('StoryName')
+	def set_Tags(self, Tags):  # Map
+		self.add_body_params("Tags", json.dumps(Tags))
+	def get_Input(self): # Struct
+		return self.get_body_params().get('Input')
+
+	def set_Input(self, Input):  # Struct
+		self.add_body_params("Input", json.dumps(Input))
+	def get_Actions(self): # Array
+		return self.get_body_params().get('Actions')
 
-	def set_StoryName(self, StoryName):  # String
-		self.add_body_params('StoryName', StoryName)
+	def set_Actions(self, Actions):  # Array
+		self.add_body_params("Actions", json.dumps(Actions))
```

### Comparing `aliyun-python-sdk-imm-2.1.16/setup.py` & `aliyun-python-sdk-imm-2.1.17/setup.py`

 * *Files identical despite different names*


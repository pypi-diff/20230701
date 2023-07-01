# Comparing `tmp/aspose-ocr-cloud-23.6.0.1.tar.gz` & `tmp/aspose-ocr-cloud-23.6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\User\source\repos\cloud.sdks\Python\python37v50\dist\.tmp-dy16isjx\aspose-ocr-cloud-23.6.0.1.tar", last modified: Sat Jul  1 19:14:32 2023, max compression
+gzip compressed data, was "C:\Users\User\source\repos\cloud.sdks\Python\python37v50\dist\.tmp-3_ufdk7o\aspose-ocr-cloud-23.6.0.2.tar", last modified: Sat Jul  1 20:15:46 2023, max compression
```

## Comparing `aspose-ocr-cloud-23.6.0.1.tar` & `aspose-ocr-cloud-23.6.0.2.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/
--rw-rw-rw-   0        0        0     1098 2023-07-01 18:23:39.000000 aspose-ocr-cloud-23.6.0.1/LICENSE
--rw-rw-rw-   0        0        0      388 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9636 2023-07-01 18:14:37.000000 aspose-ocr-cloud-23.6.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/
--rw-rw-rw-   0        0        0      734 2023-07-01 19:13:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/__init__.py
--rw-rw-rw-   0        0        0    58601 2023-07-01 19:13:45.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/api_client.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/
--rw-rw-rw-   0        0        0      214 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/__init__.py
--rw-rw-rw-   0        0        0     5630 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/path_to_api.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/
--rw-rw-rw-   0        0        0      243 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/__init__.py
--rw-rw-rw-   0        0        0      295 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_binarize_image.py
--rw-rw-rw-   0        0        0      325 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_convert_text_to_speech.py
--rw-rw-rw-   0        0        0      287 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_deskew_image.py
--rw-rw-rw-   0        0        0      295 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_detect_regions.py
--rw-rw-rw-   0        0        0      287 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_dewarp_image.py
--rw-rw-rw-   0        0        0      278 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_dj_vu2_pdf.py
--rw-rw-rw-   0        0        0      291 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_identify_font.py
--rw-rw-rw-   0        0        0      152 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_get_result_file.py
--rw-rw-rw-   0        0        0      152 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_get_result_task.py
--rw-rw-rw-   0        0        0      169 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_post_binarization_file.py
--rw-rw-rw-   0        0        0      163 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_post_dewarping_file.py
--rw-rw-rw-   0        0        0      174 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_post_skew_correction_file.py
--rw-rw-rw-   0        0        0      176 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_image_processing_post_upsampling_image_file.py
--rw-rw-rw-   0        0        0      299 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_image.py
--rw-rw-rw-   0        0        0      299 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_label.py
--rw-rw-rw-   0        0        0      291 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_pdf.py
--rw-rw-rw-   0        0        0      307 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_receipt.py
--rw-rw-rw-   0        0        0      307 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_regions.py
--rw-rw-rw-   0        0        0      299 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_recognize_table.py
--rw-rw-rw-   0        0        0      165 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_text_to_speech_get_text_to_speech_result.py
--rw-rw-rw-   0        0        0      174 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_text_to_speech_get_text_to_speech_result_file.py
--rw-rw-rw-   0        0        0      157 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_text_to_speech_post_text_to_speech.py
--rw-rw-rw-   0        0        0      291 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/paths/v5_upscale_image.py
--rw-rw-rw-   0        0        0     3082 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tag_to_api.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/
--rw-rw-rw-   0        0        0      892 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/__init__.py
--rw-rw-rw-   0        0        0      680 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/binarize_image_api.py
--rw-rw-rw-   0        0        0      746 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/convert_text_to_speech_api.py
--rw-rw-rw-   0        0        0      660 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/deskew_image_api.py
--rw-rw-rw-   0        0        0      680 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/detect_regions_api.py
--rw-rw-rw-   0        0        0      660 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/dewarp_image_api.py
--rw-rw-rw-   0        0        0      633 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/dj_vu2_pdf_api.py
--rw-rw-rw-   0        0        0      670 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/identify_font_api.py
--rw-rw-rw-   0        0        0     1116 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/image_processing_api.py
--rw-rw-rw-   0        0        0      690 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_image_api.py
--rw-rw-rw-   0        0        0      690 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_label_api.py
--rw-rw-rw-   0        0        0      670 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_pdf_api.py
--rw-rw-rw-   0        0        0      710 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_receipt_api.py
--rw-rw-rw-   0        0        0      710 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_regions_api.py
--rw-rw-rw-   0        0        0      690 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_table_api.py
--rw-rw-rw-   0        0        0      773 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/text_to_speech_api.py
--rw-rw-rw-   0        0        0      670 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/upscale_image_api.py
--rw-rw-rw-   0        0        0    16360 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/configuration.py
--rw-rw-rw-   0        0        0     4478 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/
--rw-rw-rw-   0        0        0      350 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/__init__.py
--rw-rw-rw-   0        0        0     1825 2023-07-01 17:55:01.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/dsr_confidence.py
--rw-rw-rw-   0        0        0     1931 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/dsr_mode.py
--rw-rw-rw-   0        0        0     6667 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/language.py
--rw-rw-rw-   0        0        0      928 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/language_tts.py
--rw-rw-rw-   0        0        0     2028 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_binarize_image_body.py
--rw-rw-rw-   0        0        0     2024 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_deskew_image_body.py
--rw-rw-rw-   0        0        0     2795 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_detect_regions_body.py
--rw-rw-rw-   0        0        0     2024 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_dewarp_image_body.py
--rw-rw-rw-   0        0        0     4159 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_error.py
--rw-rw-rw-   0        0        0     2795 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_font_body.py
--rw-rw-rw-   0        0        0     2859 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_image_body.py
--rw-rw-rw-   0        0        0     2805 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_label_body.py
--rw-rw-rw-   0        0        0     2847 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_pdf_body.py
--rw-rw-rw-   0        0        0     2897 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_receipt_body.py
--rw-rw-rw-   0        0        0     2825 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_regions_body.py
--rw-rw-rw-   0        0        0     2875 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_table_body.py
--rw-rw-rw-   0        0        0     4010 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_rect.py
--rw-rw-rw-   0        0        0     2671 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_region.py
--rw-rw-rw-   0        0        0     6236 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_response.py
--rw-rw-rw-   0        0        0     3836 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_result.py
--rw-rw-rw-   0        0        0    10491 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_detect_regions.py
--rw-rw-rw-   0        0        0    10481 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_dj_vu2_pdf.py
--rw-rw-rw-   0        0        0    10491 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_font.py
--rw-rw-rw-   0        0        0    10540 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_image.py
--rw-rw-rw-   0        0        0    10493 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_label.py
--rw-rw-rw-   0        0        0    10560 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_pdf.py
--rw-rw-rw-   0        0        0    10557 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_receipt.py
--rw-rw-rw-   0        0        0    10497 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_regions.py
--rw-rw-rw-   0        0        0    10546 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_table.py
--rw-rw-rw-   0        0        0     1437 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_task_status.py
--rw-rw-rw-   0        0        0     2026 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_upscale_image_body.py
--rw-rw-rw-   0        0        0     2746 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocrdj_vu2_pdf_body.py
--rw-rw-rw-   0        0        0     7870 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/problem_details.py
--rw-rw-rw-   0        0        0     1845 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/response_status_code.py
--rw-rw-rw-   0        0        0     1861 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type.py
--rw-rw-rw-   0        0        0     1318 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type_table.py
--rw-rw-rw-   0        0        0      914 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type_tts.py
--rw-rw-rw-   0        0        0     2802 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_body.py
--rw-rw-rw-   0        0        0     3523 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_body_deprecated.py
--rw-rw-rw-   0        0        0     4124 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_error.py
--rw-rw-rw-   0        0        0     6177 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_response.py
--rw-rw-rw-   0        0        0     3782 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_result.py
--rw-rw-rw-   0        0        0     2826 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_settings.py
--rw-rw-rw-   0        0        0     1420 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_task_status.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/models/
--rw-rw-rw-   0        0        0     3550 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/
--rw-rw-rw-   0        0        0     1648 2023-07-01 17:59:52.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/
--rw-rw-rw-   0        0        0      325 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/__init__.py
--rw-rw-rw-   0        0        0     8296 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/delete.py
--rw-rw-rw-   0        0        0     9917 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/get.py
--rw-rw-rw-   0        0        0    12215 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/
--rw-rw-rw-   0        0        0      341 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/__init__.py
--rw-rw-rw-   0        0        0     8388 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/delete.py
--rw-rw-rw-   0        0        0    10616 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/get.py
--rw-rw-rw-   0        0        0    12252 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/
--rw-rw-rw-   0        0        0      321 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/__init__.py
--rw-rw-rw-   0        0        0     8272 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/delete.py
--rw-rw-rw-   0        0        0     9893 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/get.py
--rw-rw-rw-   0        0        0    12177 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/
--rw-rw-rw-   0        0        0      325 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/__init__.py
--rw-rw-rw-   0        0        0     8296 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/delete.py
--rw-rw-rw-   0        0        0     9917 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/get.py
--rw-rw-rw-   0        0        0    12215 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/
--rw-rw-rw-   0        0        0      321 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/__init__.py
--rw-rw-rw-   0        0        0     8272 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/delete.py
--rw-rw-rw-   0        0        0     9893 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/get.py
--rw-rw-rw-   0        0        0    12177 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/
--rw-rw-rw-   0        0        0      316 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/__init__.py
--rw-rw-rw-   0        0        0     8246 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/delete.py
--rw-rw-rw-   0        0        0     9867 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/get.py
--rw-rw-rw-   0        0        0    12132 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/
--rw-rw-rw-   0        0        0      323 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/__init__.py
--rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/delete.py
--rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/get.py
--rw-rw-rw-   0        0        0    11618 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/
--rw-rw-rw-   0        0        0      361 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/__init__.py
--rw-rw-rw-   0        0        0    11272 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/
--rw-rw-rw-   0        0        0      361 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/__init__.py
--rw-rw-rw-   0        0        0     9881 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/
--rw-rw-rw-   0        0        0      375 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/__init__.py
--rw-rw-rw-   0        0        0    14570 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/
--rw-rw-rw-   0        0        0      369 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/__init__.py
--rw-rw-rw-   0        0        0    14528 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/
--rw-rw-rw-   0        0        0      381 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/__init__.py
--rw-rw-rw-   0        0        0    14610 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/
--rw-rw-rw-   0        0        0      383 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/__init__.py
--rw-rw-rw-   0        0        0    14547 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/
--rw-rw-rw-   0        0        0      327 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/delete.py
--rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/get.py
--rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/
--rw-rw-rw-   0        0        0      327 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/delete.py
--rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/get.py
--rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/
--rw-rw-rw-   0        0        0      323 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/__init__.py
--rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/delete.py
--rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/get.py
--rw-rw-rw-   0        0        0    12196 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/
--rw-rw-rw-   0        0        0      331 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/__init__.py
--rw-rw-rw-   0        0        0     8332 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/delete.py
--rw-rw-rw-   0        0        0     9953 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/get.py
--rw-rw-rw-   0        0        0    12272 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/
--rw-rw-rw-   0        0        0      331 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/__init__.py
--rw-rw-rw-   0        0        0     8332 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/delete.py
--rw-rw-rw-   0        0        0     9953 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/get.py
--rw-rw-rw-   0        0        0    12272 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/
--rw-rw-rw-   0        0        0      327 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/delete.py
--rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/get.py
--rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/
--rw-rw-rw-   0        0        0      377 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/__init__.py
--rw-rw-rw-   0        0        0     9997 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/
--rw-rw-rw-   0        0        0      387 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/__init__.py
--rw-rw-rw-   0        0        0    11603 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/
--rw-rw-rw-   0        0        0      365 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/__init__.py
--rw-rw-rw-   0        0        0    12195 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/
--rw-rw-rw-   0        0        0      323 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/__init__.py
--rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/delete.py
--rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/get.py
--rw-rw-rw-   0        0        0    12196 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/post.py
--rw-rw-rw-   0        0        0    10508 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/rest.py
--rw-rw-rw-   0        0        0    97618 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/schemas.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/
--rw-rw-rw-   0        0        0      388 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14093 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/example/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:54:38.000000 aspose-ocr-cloud-23.6.0.1/example/__init__.py
--rw-rw-rw-   0        0        0     1937 2023-07-01 17:36:31.000000 aspose-ocr-cloud-23.6.0.1/example/binarize_image_api_examples.py
--rw-rw-rw-   0        0        0     2113 2023-07-01 18:00:28.000000 aspose-ocr-cloud-23.6.0.1/example/convert_text_to_speech_examples.py
--rw-rw-rw-   0        0        0     2879 2023-06-29 14:30:26.000000 aspose-ocr-cloud-23.6.0.1/example/recognize_image_api_examples.py
--rw-rw-rw-   0        0        0      627 2023-07-01 18:09:29.000000 aspose-ocr-cloud-23.6.0.1/example/run.py
--rw-rw-rw-   0        0        0      643 2023-07-01 17:34:57.000000 aspose-ocr-cloud-23.6.0.1/example/utils.py
--rw-rw-rw-   0        0        0      614 2023-07-01 19:13:07.000000 aspose-ocr-cloud-23.6.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       76 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-07-01 19:13:18.000000 aspose-ocr-cloud-23.6.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/
--rw-rw-rw-   0        0        0     1214 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_binarize_image_api.py
--rw-rw-rw-   0        0        0     1320 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_convert_text_to_speech_api.py
--rw-rw-rw-   0        0        0     1184 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_deskew_image_api.py
--rw-rw-rw-   0        0        0     1214 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_detect_regions_api.py
--rw-rw-rw-   0        0        0     1184 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_dewarp_image_api.py
--rw-rw-rw-   0        0        0     1147 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.1/test/test_dj_vu2_pdf_api.py
--rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_identify_font_api.py
--rw-rw-rw-   0        0        0     1689 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_image_processing_api.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_models/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/
--rw-rw-rw-   0        0        0     1995 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/__init__.py
--rw-rw-rw-   0        0        0      862 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_delete.py
--rw-rw-rw-   0        0        0      829 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_get.py
--rw-rw-rw-   0        0        0      835 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/__init__.py
--rw-rw-rw-   0        0        0      888 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_delete.py
--rw-rw-rw-   0        0        0      855 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_get.py
--rw-rw-rw-   0        0        0      861 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/__init__.py
--rw-rw-rw-   0        0        0      854 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_delete.py
--rw-rw-rw-   0        0        0      821 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_get.py
--rw-rw-rw-   0        0        0      827 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/__init__.py
--rw-rw-rw-   0        0        0      862 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_delete.py
--rw-rw-rw-   0        0        0      829 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_get.py
--rw-rw-rw-   0        0        0      835 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/__init__.py
--rw-rw-rw-   0        0        0      854 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_delete.py
--rw-rw-rw-   0        0        0      821 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_get.py
--rw-rw-rw-   0        0        0      827 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/__init__.py
--rw-rw-rw-   0        0        0      843 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_delete.py
--rw-rw-rw-   0        0        0      810 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_get.py
--rw-rw-rw-   0        0        0      816 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_delete.py
--rw-rw-rw-   0        0        0      825 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_get.py
--rw-rw-rw-   0        0        0      831 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_file/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_file/test_get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_task/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_task/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_task/test_get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_binarization_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_binarization_file/__init__.py
--rw-rw-rw-   0        0        0      905 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_binarization_file/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_dewarping_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_dewarping_file/__init__.py
--rw-rw-rw-   0        0        0      893 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_dewarping_file/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_skew_correction_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_skew_correction_file/__init__.py
--rw-rw-rw-   0        0        0      914 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_skew_correction_file/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:31.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_upsampling_image_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_upsampling_image_file/__init__.py
--rw-rw-rw-   0        0        0      918 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_upsampling_image_file/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/__init__.py
--rw-rw-rw-   0        0        0      866 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_delete.py
--rw-rw-rw-   0        0        0      833 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_get.py
--rw-rw-rw-   0        0        0      839 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/__init__.py
--rw-rw-rw-   0        0        0      866 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_delete.py
--rw-rw-rw-   0        0        0      833 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_get.py
--rw-rw-rw-   0        0        0      839 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_delete.py
--rw-rw-rw-   0        0        0      825 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_get.py
--rw-rw-rw-   0        0        0      831 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_delete.py
--rw-rw-rw-   0        0        0      841 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_get.py
--rw-rw-rw-   0        0        0      847 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/__init__.py
--rw-rw-rw-   0        0        0      874 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_delete.py
--rw-rw-rw-   0        0        0      841 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_get.py
--rw-rw-rw-   0        0        0      847 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/__init__.py
--rw-rw-rw-   0        0        0      866 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_delete.py
--rw-rw-rw-   0        0        0      833 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_get.py
--rw-rw-rw-   0        0        0      839 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/__init__.py
--rw-rw-rw-   0        0        0      900 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/test_get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/__init__.py
--rw-rw-rw-   0        0        0      917 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/test_get.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_post_text_to_speech/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_post_text_to_speech/__init__.py
--rw-rw-rw-   0        0        0      884 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_post_text_to_speech/test_post.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:14:32.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/
--rw-rw-rw-   0        0        0        0 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/__init__.py
--rw-rw-rw-   0        0        0      858 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_delete.py
--rw-rw-rw-   0        0        0      825 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_get.py
--rw-rw-rw-   0        0        0      831 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_post.py
--rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_image_api.py
--rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_label_api.py
--rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_pdf_api.py
--rw-rw-rw-   0        0        0     1259 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_receipt_api.py
--rw-rw-rw-   0        0        0     1259 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_regions_api.py
--rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_recognize_table_api.py
--rw-rw-rw-   0        0        0     1252 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_text_to_speech_api.py
--rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.1/test/test_upscale_image_api.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/
+-rw-rw-rw-   0        0        0     1098 2023-07-01 18:23:39.000000 aspose-ocr-cloud-23.6.0.2/LICENSE
+-rw-rw-rw-   0        0        0    10132 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9636 2023-07-01 18:14:37.000000 aspose-ocr-cloud-23.6.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/
+-rw-rw-rw-   0        0        0      734 2023-07-01 19:42:32.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/__init__.py
+-rw-rw-rw-   0        0        0    58599 2023-07-01 20:14:06.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/api_client.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/
+-rw-rw-rw-   0        0        0      214 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/__init__.py
+-rw-rw-rw-   0        0        0     5630 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/path_to_api.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/
+-rw-rw-rw-   0        0        0      243 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/__init__.py
+-rw-rw-rw-   0        0        0      295 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_binarize_image.py
+-rw-rw-rw-   0        0        0      325 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_convert_text_to_speech.py
+-rw-rw-rw-   0        0        0      287 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_deskew_image.py
+-rw-rw-rw-   0        0        0      295 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_detect_regions.py
+-rw-rw-rw-   0        0        0      287 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_dewarp_image.py
+-rw-rw-rw-   0        0        0      278 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_dj_vu2_pdf.py
+-rw-rw-rw-   0        0        0      291 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_identify_font.py
+-rw-rw-rw-   0        0        0      152 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_get_result_file.py
+-rw-rw-rw-   0        0        0      152 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_get_result_task.py
+-rw-rw-rw-   0        0        0      169 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_post_binarization_file.py
+-rw-rw-rw-   0        0        0      163 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_post_dewarping_file.py
+-rw-rw-rw-   0        0        0      174 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_post_skew_correction_file.py
+-rw-rw-rw-   0        0        0      176 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_image_processing_post_upsampling_image_file.py
+-rw-rw-rw-   0        0        0      299 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_image.py
+-rw-rw-rw-   0        0        0      299 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_label.py
+-rw-rw-rw-   0        0        0      291 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_pdf.py
+-rw-rw-rw-   0        0        0      307 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_receipt.py
+-rw-rw-rw-   0        0        0      307 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_regions.py
+-rw-rw-rw-   0        0        0      299 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_recognize_table.py
+-rw-rw-rw-   0        0        0      165 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_text_to_speech_get_text_to_speech_result.py
+-rw-rw-rw-   0        0        0      174 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_text_to_speech_get_text_to_speech_result_file.py
+-rw-rw-rw-   0        0        0      157 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_text_to_speech_post_text_to_speech.py
+-rw-rw-rw-   0        0        0      291 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/paths/v5_upscale_image.py
+-rw-rw-rw-   0        0        0     3082 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tag_to_api.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/
+-rw-rw-rw-   0        0        0      892 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/binarize_image_api.py
+-rw-rw-rw-   0        0        0      746 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/convert_text_to_speech_api.py
+-rw-rw-rw-   0        0        0      660 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/deskew_image_api.py
+-rw-rw-rw-   0        0        0      680 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/detect_regions_api.py
+-rw-rw-rw-   0        0        0      660 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/dewarp_image_api.py
+-rw-rw-rw-   0        0        0      633 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/dj_vu2_pdf_api.py
+-rw-rw-rw-   0        0        0      670 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/identify_font_api.py
+-rw-rw-rw-   0        0        0     1116 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/image_processing_api.py
+-rw-rw-rw-   0        0        0      690 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_image_api.py
+-rw-rw-rw-   0        0        0      690 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_label_api.py
+-rw-rw-rw-   0        0        0      670 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_pdf_api.py
+-rw-rw-rw-   0        0        0      710 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_receipt_api.py
+-rw-rw-rw-   0        0        0      710 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_regions_api.py
+-rw-rw-rw-   0        0        0      690 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_table_api.py
+-rw-rw-rw-   0        0        0      773 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/text_to_speech_api.py
+-rw-rw-rw-   0        0        0      670 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/upscale_image_api.py
+-rw-rw-rw-   0        0        0    16362 2023-07-01 19:42:31.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/configuration.py
+-rw-rw-rw-   0        0        0     4478 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/
+-rw-rw-rw-   0        0        0      350 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/__init__.py
+-rw-rw-rw-   0        0        0     1825 2023-07-01 17:55:01.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/dsr_confidence.py
+-rw-rw-rw-   0        0        0     1931 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/dsr_mode.py
+-rw-rw-rw-   0        0        0     6667 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/language.py
+-rw-rw-rw-   0        0        0      928 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/language_tts.py
+-rw-rw-rw-   0        0        0     2028 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_binarize_image_body.py
+-rw-rw-rw-   0        0        0     2024 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_deskew_image_body.py
+-rw-rw-rw-   0        0        0     2795 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_detect_regions_body.py
+-rw-rw-rw-   0        0        0     2024 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_dewarp_image_body.py
+-rw-rw-rw-   0        0        0     4159 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_error.py
+-rw-rw-rw-   0        0        0     2795 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_font_body.py
+-rw-rw-rw-   0        0        0     2859 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_image_body.py
+-rw-rw-rw-   0        0        0     2805 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_label_body.py
+-rw-rw-rw-   0        0        0     2847 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_pdf_body.py
+-rw-rw-rw-   0        0        0     2897 2023-07-01 17:55:03.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_receipt_body.py
+-rw-rw-rw-   0        0        0     2825 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_regions_body.py
+-rw-rw-rw-   0        0        0     2875 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_table_body.py
+-rw-rw-rw-   0        0        0     4010 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_rect.py
+-rw-rw-rw-   0        0        0     2671 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_region.py
+-rw-rw-rw-   0        0        0     6236 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_response.py
+-rw-rw-rw-   0        0        0     3836 2023-07-01 17:55:04.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_result.py
+-rw-rw-rw-   0        0        0    10491 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_detect_regions.py
+-rw-rw-rw-   0        0        0    10481 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_dj_vu2_pdf.py
+-rw-rw-rw-   0        0        0    10491 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_font.py
+-rw-rw-rw-   0        0        0    10540 2023-07-01 17:55:05.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_image.py
+-rw-rw-rw-   0        0        0    10493 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_label.py
+-rw-rw-rw-   0        0        0    10560 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_pdf.py
+-rw-rw-rw-   0        0        0    10557 2023-07-01 17:55:06.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_receipt.py
+-rw-rw-rw-   0        0        0    10497 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_regions.py
+-rw-rw-rw-   0        0        0    10546 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_table.py
+-rw-rw-rw-   0        0        0     1437 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_task_status.py
+-rw-rw-rw-   0        0        0     2026 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_upscale_image_body.py
+-rw-rw-rw-   0        0        0     2746 2023-07-01 17:55:02.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocrdj_vu2_pdf_body.py
+-rw-rw-rw-   0        0        0     7870 2023-07-01 17:55:07.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/problem_details.py
+-rw-rw-rw-   0        0        0     1845 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/response_status_code.py
+-rw-rw-rw-   0        0        0     1861 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type.py
+-rw-rw-rw-   0        0        0     1318 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type_table.py
+-rw-rw-rw-   0        0        0      914 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type_tts.py
+-rw-rw-rw-   0        0        0     2802 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_body.py
+-rw-rw-rw-   0        0        0     3523 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_body_deprecated.py
+-rw-rw-rw-   0        0        0     4124 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_error.py
+-rw-rw-rw-   0        0        0     6177 2023-07-01 17:55:08.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_response.py
+-rw-rw-rw-   0        0        0     3782 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_result.py
+-rw-rw-rw-   0        0        0     2826 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_settings.py
+-rw-rw-rw-   0        0        0     1420 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_task_status.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/models/
+-rw-rw-rw-   0        0        0     3550 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/
+-rw-rw-rw-   0        0        0     1648 2023-07-01 17:59:52.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/
+-rw-rw-rw-   0        0        0      325 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/__init__.py
+-rw-rw-rw-   0        0        0     8296 2023-07-01 17:55:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/delete.py
+-rw-rw-rw-   0        0        0     9917 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/get.py
+-rw-rw-rw-   0        0        0    12215 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/
+-rw-rw-rw-   0        0        0      341 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0     8388 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/delete.py
+-rw-rw-rw-   0        0        0    10616 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/get.py
+-rw-rw-rw-   0        0        0    12252 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/
+-rw-rw-rw-   0        0        0      321 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/__init__.py
+-rw-rw-rw-   0        0        0     8272 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/delete.py
+-rw-rw-rw-   0        0        0     9893 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/get.py
+-rw-rw-rw-   0        0        0    12177 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/
+-rw-rw-rw-   0        0        0      325 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/__init__.py
+-rw-rw-rw-   0        0        0     8296 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/delete.py
+-rw-rw-rw-   0        0        0     9917 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/get.py
+-rw-rw-rw-   0        0        0    12215 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/
+-rw-rw-rw-   0        0        0      321 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/__init__.py
+-rw-rw-rw-   0        0        0     8272 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/delete.py
+-rw-rw-rw-   0        0        0     9893 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/get.py
+-rw-rw-rw-   0        0        0    12177 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/
+-rw-rw-rw-   0        0        0      316 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/__init__.py
+-rw-rw-rw-   0        0        0     8246 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/delete.py
+-rw-rw-rw-   0        0        0     9867 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/get.py
+-rw-rw-rw-   0        0        0    12132 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/
+-rw-rw-rw-   0        0        0      323 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/__init__.py
+-rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/delete.py
+-rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/get.py
+-rw-rw-rw-   0        0        0    11618 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/
+-rw-rw-rw-   0        0        0      361 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/__init__.py
+-rw-rw-rw-   0        0        0    11272 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/
+-rw-rw-rw-   0        0        0      361 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/__init__.py
+-rw-rw-rw-   0        0        0     9881 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/
+-rw-rw-rw-   0        0        0      375 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/__init__.py
+-rw-rw-rw-   0        0        0    14570 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/
+-rw-rw-rw-   0        0        0      369 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/__init__.py
+-rw-rw-rw-   0        0        0    14528 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/
+-rw-rw-rw-   0        0        0      381 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/__init__.py
+-rw-rw-rw-   0        0        0    14610 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/
+-rw-rw-rw-   0        0        0      383 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/__init__.py
+-rw-rw-rw-   0        0        0    14547 2023-07-01 17:58:09.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/
+-rw-rw-rw-   0        0        0      327 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/delete.py
+-rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/get.py
+-rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/
+-rw-rw-rw-   0        0        0      327 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/delete.py
+-rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/get.py
+-rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/
+-rw-rw-rw-   0        0        0      323 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/__init__.py
+-rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/delete.py
+-rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/get.py
+-rw-rw-rw-   0        0        0    12196 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/
+-rw-rw-rw-   0        0        0      331 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/__init__.py
+-rw-rw-rw-   0        0        0     8332 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/delete.py
+-rw-rw-rw-   0        0        0     9953 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/get.py
+-rw-rw-rw-   0        0        0    12272 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/
+-rw-rw-rw-   0        0        0      331 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/__init__.py
+-rw-rw-rw-   0        0        0     8332 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/delete.py
+-rw-rw-rw-   0        0        0     9953 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/get.py
+-rw-rw-rw-   0        0        0    12272 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/
+-rw-rw-rw-   0        0        0      327 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/delete.py
+-rw-rw-rw-   0        0        0     9929 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/get.py
+-rw-rw-rw-   0        0        0    12234 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/
+-rw-rw-rw-   0        0        0      377 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/__init__.py
+-rw-rw-rw-   0        0        0     9997 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/
+-rw-rw-rw-   0        0        0      387 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/__init__.py
+-rw-rw-rw-   0        0        0    11603 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/
+-rw-rw-rw-   0        0        0      365 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0    12195 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/
+-rw-rw-rw-   0        0        0      323 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/__init__.py
+-rw-rw-rw-   0        0        0     8284 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/delete.py
+-rw-rw-rw-   0        0        0     9905 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/get.py
+-rw-rw-rw-   0        0        0    12196 2023-07-01 17:58:26.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/post.py
+-rw-rw-rw-   0        0        0    10508 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/rest.py
+-rw-rw-rw-   0        0        0    97618 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/schemas.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/
+-rw-rw-rw-   0        0        0    10132 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14093 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/example/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:54:38.000000 aspose-ocr-cloud-23.6.0.2/example/__init__.py
+-rw-rw-rw-   0        0        0     1937 2023-07-01 17:36:31.000000 aspose-ocr-cloud-23.6.0.2/example/binarize_image_api_examples.py
+-rw-rw-rw-   0        0        0     2113 2023-07-01 18:00:28.000000 aspose-ocr-cloud-23.6.0.2/example/convert_text_to_speech_examples.py
+-rw-rw-rw-   0        0        0     2879 2023-06-29 14:30:26.000000 aspose-ocr-cloud-23.6.0.2/example/recognize_image_api_examples.py
+-rw-rw-rw-   0        0        0      627 2023-07-01 18:09:29.000000 aspose-ocr-cloud-23.6.0.2/example/run.py
+-rw-rw-rw-   0        0        0      643 2023-07-01 17:34:57.000000 aspose-ocr-cloud-23.6.0.2/example/utils.py
+-rw-rw-rw-   0        0        0      584 2023-07-01 20:13:32.000000 aspose-ocr-cloud-23.6.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       76 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-07-01 20:14:38.000000 aspose-ocr-cloud-23.6.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/
+-rw-rw-rw-   0        0        0     1214 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_binarize_image_api.py
+-rw-rw-rw-   0        0        0     1320 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_convert_text_to_speech_api.py
+-rw-rw-rw-   0        0        0     1184 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_deskew_image_api.py
+-rw-rw-rw-   0        0        0     1214 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_detect_regions_api.py
+-rw-rw-rw-   0        0        0     1184 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_dewarp_image_api.py
+-rw-rw-rw-   0        0        0     1147 2023-06-28 20:56:55.000000 aspose-ocr-cloud-23.6.0.2/test/test_dj_vu2_pdf_api.py
+-rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_identify_font_api.py
+-rw-rw-rw-   0        0        0     1689 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_image_processing_api.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_models/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/
+-rw-rw-rw-   0        0        0     1995 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/__init__.py
+-rw-rw-rw-   0        0        0      862 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_delete.py
+-rw-rw-rw-   0        0        0      829 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_get.py
+-rw-rw-rw-   0        0        0      835 2023-07-01 17:55:10.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_delete.py
+-rw-rw-rw-   0        0        0      855 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_get.py
+-rw-rw-rw-   0        0        0      861 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_delete.py
+-rw-rw-rw-   0        0        0      821 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_get.py
+-rw-rw-rw-   0        0        0      827 2023-07-01 17:55:11.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/__init__.py
+-rw-rw-rw-   0        0        0      862 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_delete.py
+-rw-rw-rw-   0        0        0      829 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_get.py
+-rw-rw-rw-   0        0        0      835 2023-07-01 17:55:12.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_delete.py
+-rw-rw-rw-   0        0        0      821 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_get.py
+-rw-rw-rw-   0        0        0      827 2023-07-01 17:55:13.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/__init__.py
+-rw-rw-rw-   0        0        0      843 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_delete.py
+-rw-rw-rw-   0        0        0      810 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_get.py
+-rw-rw-rw-   0        0        0      816 2023-07-01 17:55:14.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_delete.py
+-rw-rw-rw-   0        0        0      825 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_get.py
+-rw-rw-rw-   0        0        0      831 2023-07-01 17:55:15.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_file/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_file/test_get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_task/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_task/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_task/test_get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_binarization_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_binarization_file/__init__.py
+-rw-rw-rw-   0        0        0      905 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_binarization_file/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_dewarping_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_dewarping_file/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_dewarping_file/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_skew_correction_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_skew_correction_file/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_skew_correction_file/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_upsampling_image_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_upsampling_image_file/__init__.py
+-rw-rw-rw-   0        0        0      918 2023-07-01 17:55:17.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_upsampling_image_file/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/__init__.py
+-rw-rw-rw-   0        0        0      866 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_delete.py
+-rw-rw-rw-   0        0        0      833 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_get.py
+-rw-rw-rw-   0        0        0      839 2023-07-01 17:55:18.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/__init__.py
+-rw-rw-rw-   0        0        0      866 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_delete.py
+-rw-rw-rw-   0        0        0      833 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_get.py
+-rw-rw-rw-   0        0        0      839 2023-07-01 17:55:19.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_delete.py
+-rw-rw-rw-   0        0        0      825 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_get.py
+-rw-rw-rw-   0        0        0      831 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_delete.py
+-rw-rw-rw-   0        0        0      841 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_get.py
+-rw-rw-rw-   0        0        0      847 2023-07-01 17:55:20.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/__init__.py
+-rw-rw-rw-   0        0        0      874 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_delete.py
+-rw-rw-rw-   0        0        0      841 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_get.py
+-rw-rw-rw-   0        0        0      847 2023-07-01 17:55:21.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/__init__.py
+-rw-rw-rw-   0        0        0      866 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_delete.py
+-rw-rw-rw-   0        0        0      833 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_get.py
+-rw-rw-rw-   0        0        0      839 2023-07-01 17:55:22.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/test_get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/__init__.py
+-rw-rw-rw-   0        0        0      917 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/test_get.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_post_text_to_speech/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_post_text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0      884 2023-07-01 17:55:23.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_post_text_to_speech/test_post.py
+drwxrwxrwx   0        0        0        0 2023-07-01 20:15:46.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/
+-rw-rw-rw-   0        0        0        0 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_delete.py
+-rw-rw-rw-   0        0        0      825 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_get.py
+-rw-rw-rw-   0        0        0      831 2023-07-01 17:55:24.000000 aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_post.py
+-rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_image_api.py
+-rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_label_api.py
+-rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_pdf_api.py
+-rw-rw-rw-   0        0        0     1259 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_receipt_api.py
+-rw-rw-rw-   0        0        0     1259 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_regions_api.py
+-rw-rw-rw-   0        0        0     1229 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_recognize_table_api.py
+-rw-rw-rw-   0        0        0     1252 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_text_to_speech_api.py
+-rw-rw-rw-   0        0        0     1199 2023-06-28 20:56:56.000000 aspose-ocr-cloud-23.6.0.2/test/test_upscale_image_api.py
```

### Comparing `aspose-ocr-cloud-23.6.0.1/LICENSE` & `aspose-ocr-cloud-23.6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/README.md` & `aspose-ocr-cloud-23.6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/__init__.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Aspose OCR Cloud 5.0 API  # noqa: E501
 
     The version of the OpenAPI document: 5.0
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "23.6.0.1"
+__version__ = "23.6.0.2"
 
 # import ApiClient
 from aspose_ocr_cloud.api_client import ApiClient
 
 # import Configuration
 from aspose_ocr_cloud.configuration import Configuration
```

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/api_client.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/23.6.0.1/python'
+        self.user_agent = 'OpenAPI-Generator/23.6.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/path_to_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tag_to_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/__init__.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/binarize_image_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/binarize_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/convert_text_to_speech_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/convert_text_to_speech_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/deskew_image_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/deskew_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/detect_regions_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/detect_regions_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/dewarp_image_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/dewarp_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/dj_vu2_pdf_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/dj_vu2_pdf_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/identify_font_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/identify_font_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/image_processing_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/image_processing_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_image_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_label_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_label_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_pdf_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_pdf_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_receipt_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_receipt_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_regions_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_regions_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/recognize_table_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/recognize_table_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/text_to_speech_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/text_to_speech_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/apis/tags/upscale_image_api.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/apis/tags/upscale_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/configuration.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 5.0\n"\
-               "SDK Package Version: 23.6.0".\
+               "SDK Package Version: 23.6.0.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/exceptions.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/dsr_confidence.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/dsr_confidence.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/dsr_mode.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/dsr_mode.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/language.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/language.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/language_tts.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/language_tts.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_binarize_image_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_binarize_image_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_deskew_image_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_deskew_image_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_detect_regions_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_detect_regions_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_dewarp_image_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_dewarp_image_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_error.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_error.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_font_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_font_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_image_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_image_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_label_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_label_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_pdf_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_pdf_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_receipt_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_receipt_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_regions_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_regions_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_recognize_table_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_recognize_table_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_rect.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_rect.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_region.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_region.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_response.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_response.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_result.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_result.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_detect_regions.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_detect_regions.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_dj_vu2_pdf.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_dj_vu2_pdf.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_font.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_font.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_image.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_image.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_label.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_label.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_pdf.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_pdf.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_receipt.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_receipt.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_regions.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_regions.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_settings_recognize_table.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_settings_recognize_table.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_task_status.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_task_status.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocr_upscale_image_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocr_upscale_image_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/ocrdj_vu2_pdf_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/ocrdj_vu2_pdf_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/problem_details.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/response_status_code.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/response_status_code.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type_table.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type_table.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/result_type_tts.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/result_type_tts.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_body.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_body.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_body_deprecated.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_body_deprecated.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_error.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_error.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_response.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_result.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_result.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_settings.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_settings.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/model/tts_task_status.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/model/tts_task_status.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/models/__init__.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/__init__.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_binarize_image/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_binarize_image/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_convert_text_to_speech/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_convert_text_to_speech/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_deskew_image/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_deskew_image/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_detect_regions/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_detect_regions/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dewarp_image/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dewarp_image/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_dj_vu2_pdf/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_identify_font/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_identify_font/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_file/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_get_result_task/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_binarization_file/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_dewarping_file/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_skew_correction_file/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_image_processing_post_upsampling_image_file/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_image/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_image/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_label/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_label/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_pdf/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_pdf/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_receipt/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_receipt/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_regions/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_regions/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_recognize_table/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_recognize_table/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_get_text_to_speech_result_file/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_text_to_speech_post_text_to_speech/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/delete.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/get.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/paths/v5_upscale_image/post.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/paths/v5_upscale_image/post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/rest.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud/schemas.py` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud/schemas.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/aspose_ocr_cloud.egg-info/SOURCES.txt` & `aspose-ocr-cloud-23.6.0.2/aspose_ocr_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/example/binarize_image_api_examples.py` & `aspose-ocr-cloud-23.6.0.2/example/binarize_image_api_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/example/convert_text_to_speech_examples.py` & `aspose-ocr-cloud-23.6.0.2/example/convert_text_to_speech_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/example/recognize_image_api_examples.py` & `aspose-ocr-cloud-23.6.0.2/example/recognize_image_api_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/example/run.py` & `aspose-ocr-cloud-23.6.0.2/example/run.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/example/utils.py` & `aspose-ocr-cloud-23.6.0.2/example/utils.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/setup.py` & `aspose-ocr-cloud-23.6.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The version of the OpenAPI document: 5.0
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "aspose-ocr-cloud"
-VERSION = "23.6.0.1"
+VERSION = "23.6.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -25,24 +25,28 @@
     "frozendict ~= 2.3.4",
     "python-dateutil ~= 2.7.0",
     "setuptools >= 21.0.0",
     "typing_extensions ~= 4.3.0",
     "urllib3 ~= 1.26.7",
 ]
 
+# read the contents of README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name=NAME,
     version=VERSION,
     description="Aspose OCR Cloud 5.0 API",
     author="Aspose",
-    author_email="team@openapitools.org",
+    author_email="",
     url="https://pypi.org/project/aspose-ocr-cloud/",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Aspose OCR Cloud 5.0 API"],
+    keywords=["Aspose", "OCR", "Aspose OCR Cloud 5.0 API"],
     python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
-    license="License",
-    long_description="""\
-    Aspose OCR Cloud 5.0 API  # noqa: E501
-    """
+    license="MIT",
+    long_description_content_type="text/markdown",
+    long_description=long_description
 )
```

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_binarize_image_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_binarize_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_convert_text_to_speech_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_convert_text_to_speech_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_deskew_image_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_deskew_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_detect_regions_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_detect_regions_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_dewarp_image_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_dewarp_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_dj_vu2_pdf_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_dj_vu2_pdf_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_identify_font_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_identify_font_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_image_processing_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_image_processing_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/__init__.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_binarize_image/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_binarize_image/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_convert_text_to_speech/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_convert_text_to_speech/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_deskew_image/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_deskew_image/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_detect_regions/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_detect_regions/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dewarp_image/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dewarp_image/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_dj_vu2_pdf/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_dj_vu2_pdf/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_identify_font/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_identify_font/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_file/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_file/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_get_result_task/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_get_result_task/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_binarization_file/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_binarization_file/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_dewarping_file/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_dewarping_file/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_skew_correction_file/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_skew_correction_file/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_image_processing_post_upsampling_image_file/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_image_processing_post_upsampling_image_file/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_image/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_image/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_label/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_label/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_pdf/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_pdf/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_receipt/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_receipt/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_regions/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_regions/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_recognize_table/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_recognize_table/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_get_text_to_speech_result_file/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_text_to_speech_post_text_to_speech/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_text_to_speech_post_text_to_speech/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_delete.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_delete.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_get.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_get.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_paths/test_v5_upscale_image/test_post.py` & `aspose-ocr-cloud-23.6.0.2/test/test_paths/test_v5_upscale_image/test_post.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_image_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_image_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_label_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_label_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_pdf_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_pdf_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_receipt_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_receipt_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_regions_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_regions_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_recognize_table_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_recognize_table_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_text_to_speech_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_text_to_speech_api.py`

 * *Files identical despite different names*

### Comparing `aspose-ocr-cloud-23.6.0.1/test/test_upscale_image_api.py` & `aspose-ocr-cloud-23.6.0.2/test/test_upscale_image_api.py`

 * *Files identical despite different names*


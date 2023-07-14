# Comparing `tmp/aspose-words-cloud-23.5.1.tar.gz` & `tmp/aspose-words-cloud-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aspose-words-cloud-23.5.1.tar", last modified: Thu Jun 29 06:03:27 2023, max compression
+gzip compressed data, was "dist/aspose-words-cloud-23.6.0.tar", last modified: Fri Jul 14 07:46:02 2023, max compression
```

## Comparing `aspose-words-cloud-23.5.1.tar` & `aspose-words-cloud-23.6.0.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12523 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/test/
--rw-r--r--   0 root         (0) root         (0)     3484 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/base_test_context.py
--rw-r--r--   0 root         (0) root         (0)     9634 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/test_batch.py
--rw-r--r--   0 root         (0) root         (0)     3318 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/test_examples.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/test_url_encode.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/test_doc_with_password.py
--rw-r--r--   0 root         (0) root         (0)     4054 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/test/test_readme.py
--rw-r--r--   0 root         (0) root         (0)    13759 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2228 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/asposewordscloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/
--rw-r--r--   0 root         (0) root         (0)    11024 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style_apply.py
--rw-r--r--   0 root         (0) root         (0)    45668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/jpeg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_parts_response.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_insert.py
--rw-r--r--   0 root         (0) root         (0)     6354 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_response.py
--rw-r--r--   0 root         (0) root         (0)     8614 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/csv_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bmp_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    24397 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/word_ml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6694 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_response.py
--rw-r--r--   0 root         (0) root         (0)     6444 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_levels.py
--rw-r--r--   0 root         (0) root         (0)     6538 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks_response.py
--rw-r--r--   0 root         (0) root         (0)     6915 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_objects_response.py
--rw-r--r--   0 root         (0) root         (0)     6467 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/lists_response.py
--rw-r--r--   0 root         (0) root         (0)    14309 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_insert.py
--rw-r--r--   0 root         (0) root         (0)     6411 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_collection.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_object_response.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/fields_response.py
--rw-r--r--   0 root         (0) root         (0)     7306 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/image_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    27747 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/dot_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     8276 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_entry.py
--rw-r--r--   0 root         (0) root         (0)    23377 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style.py
--rw-r--r--   0 root         (0) root         (0)     7026 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_link.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/dotx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    50657 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/tiff_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/save_response.py
--rw-r--r--   0 root         (0) root         (0)     6292 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/run_response.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_response.py
--rw-r--r--   0 root         (0) root         (0)    76376 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/epub_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_list_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/new_document_position.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xml_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     8924 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_update.py
--rw-r--r--   0 root         (0) root         (0)    28013 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/ott_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7126 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell.py
--rw-r--r--   0 root         (0) root         (0)     6550 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_objects_collection.py
--rw-r--r--   0 root         (0) root         (0)     6767 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     4838 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format_dto.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlinks_response.py
--rw-r--r--   0 root         (0) root         (0)     6779 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks_outline_level_data.py
--rw-r--r--   0 root         (0) root         (0)    13381 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_update.py
--rw-r--r--   0 root         (0) root         (0)    34808 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_update.py
--rw-r--r--   0 root         (0) root         (0)     7124 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph.py
--rw-r--r--   0 root         (0) root         (0)     6565 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnotes_response.py
--rw-r--r--   0 root         (0) root         (0)     7537 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/split_document_result.py
--rw-r--r--   0 root         (0) root         (0)    19100 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format.py
--rw-r--r--   0 root         (0) root         (0)     7099 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tags_response.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_response.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section_page_setup_response.py
--rw-r--r--   0 root         (0) root         (0)     6496 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlink_response.py
--rw-r--r--   0 root         (0) root         (0)     8434 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field.py
--rw-r--r--   0 root         (0) root         (0)     9407 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer.py
--rw-r--r--   0 root         (0) root         (0)     6524 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stops_response.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_response.py
--rw-r--r--   0 root         (0) root         (0)     6494 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_response.py
--rw-r--r--   0 root         (0) root         (0)    40523 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/page_setup.py
--rw-r--r--   0 root         (0) root         (0)    28040 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_data.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comment_response.py
--rw-r--r--   0 root         (0) root         (0)    30577 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/markdown_save_options_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_header_footer_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_page_numbers_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/compress_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/compare_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_section_page_setup_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/protect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1724 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_run_font_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_fields_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/replace_with_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/replace_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_row_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/reject_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_row_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_paragraph_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_borders_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/remove_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_bookmark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/accept_all_revisions_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_footnote_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1705 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     7176 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_comment_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_run_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1693 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_cell_format_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_tiff_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_list_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/unprotect_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_form_field_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_border_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_range_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_properties_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/split_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_paragraph_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/copy_style_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_list_level_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_watermark_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_cell_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_drawing_object_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_watermark_text_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/append_document_online_response.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_watermark_image_online_response.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/docm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    32952 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/ps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6525 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comments_collection.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/dotm_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_response.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop.py
--rw-r--r--   0 root         (0) root         (0)     6621 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlinks.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_link.py
--rw-r--r--   0 root         (0) root         (0)     6248 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xml_color.py
--rw-r--r--   0 root         (0) root         (0)     7024 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_update.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_response.py
--rw-r--r--   0 root         (0) root         (0)    34159 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/font_response.py
--rw-r--r--   0 root         (0) root         (0)     6496 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_response.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_collection.py
--rw-r--r--   0 root         (0) root         (0)     7608 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     5761 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/range_document_dto.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_response.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comment_link.py
--rw-r--r--   0 root         (0) root         (0)     8999 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/file_link.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/node_link.py
--rw-r--r--   0 root         (0) root         (0)     7697 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/protection_data_response.py
--rw-r--r--   0 root         (0) root         (0)    34808 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_insert.py
--rw-r--r--   0 root         (0) root         (0)    16483 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/compare_options.py
--rw-r--r--   0 root         (0) root         (0)     6817 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/load_web_document_data.py
--rw-r--r--   0 root         (0) root         (0)     8854 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style_update.py
--rw-r--r--   0 root         (0) root         (0)     5256 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/report_build_options.py
--rw-r--r--   0 root         (0) root         (0)     6388 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/range_text_response.py
--rw-r--r--   0 root         (0) root         (0)     6773 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)    11839 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/report_engine_settings.py
--rw-r--r--   0 root         (0) root         (0)     6464 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/words_api_error_response.py
--rw-r--r--   0 root         (0) root         (0)     6389 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_collection.py
--rw-r--r--   0 root         (0) root         (0)     7072 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style_insert.py
--rw-r--r--   0 root         (0) root         (0)     5596 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_link.py
--rw-r--r--   0 root         (0) root         (0)     8058 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table.py
--rw-r--r--   0 root         (0) root         (0)     6730 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_insert.py
--rw-r--r--   0 root         (0) root         (0)     6721 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/modification_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     6810 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_parts_collection.py
--rw-r--r--   0 root         (0) root         (0)    17850 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_checkbox.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section_link_collection_response.py
--rw-r--r--   0 root         (0) root         (0)     5736 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/range_document.py
--rw-r--r--   0 root         (0) root         (0)     5739 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/story_child_nodes.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_collection.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link.py
--rw-r--r--   0 root         (0) root         (0)     6691 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/split_document_response.py
--rw-r--r--   0 root         (0) root         (0)     6366 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_link.py
--rw-r--r--   0 root         (0) root         (0)     8453 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/downsample_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10167 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_digital_signature_details_data.py
--rw-r--r--   0 root         (0) root         (0)     6775 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_objects_response.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format.py
--rw-r--r--   0 root         (0) root         (0)     7673 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/save_result.py
--rw-r--r--   0 root         (0) root         (0)     8245 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop_insert.py
--rw-r--r--   0 root         (0) root         (0)    36909 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/open_xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6397 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/optimization_options.py
--rw-r--r--   0 root         (0) root         (0)     6788 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/replace_range_dto.py
--rw-r--r--   0 root         (0) root         (0)    12026 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_object.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/styles_response.py
--rw-r--r--   0 root         (0) root         (0)     5795 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/protection_data.py
--rw-r--r--   0 root         (0) root         (0)    28658 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     5915 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/image_entry.py
--rw-r--r--   0 root         (0) root         (0)    11051 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comment.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/compress_response.py
--rw-r--r--   0 root         (0) root         (0)    28017 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/odt_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6117 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_update.py
--rw-r--r--   0 root         (0) root         (0)    16964 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_drop_down.py
--rw-r--r--   0 root         (0) root         (0)    12508 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_info.py
--rw-r--r--   0 root         (0) root         (0)     8786 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/classification_response.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format_response.py
--rw-r--r--   0 root         (0) root         (0)     9566 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/compare_data.py
--rw-r--r--   0 root         (0) root         (0)    28036 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/rtf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6468 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/watermark_text.py
--rw-r--r--   0 root         (0) root         (0)     8079 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_property.py
--rw-r--r--   0 root         (0) root         (0)     6220 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/info_additional_item.py
--rw-r--r--   0 root         (0) root         (0)     6350 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/borders_collection.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_collection.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/classification_result.py
--rw-r--r--   0 root         (0) root         (0)    75129 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/html_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    34704 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6770 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comments_response.py
--rw-r--r--   0 root         (0) root         (0)    38869 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/svg_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    28886 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_template_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/gif_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/borders_response.py
--rw-r--r--   0 root         (0) root         (0)     6773 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/header_footers_response.py
--rw-r--r--   0 root         (0) root         (0)    36496 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xps_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    18821 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_level.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/run_insert.py
--rw-r--r--   0 root         (0) root         (0)    67826 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     5704 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style_copy.py
--rw-r--r--   0 root         (0) root         (0)    17661 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object.py
--rw-r--r--   0 root         (0) root         (0)     6846 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/revisions_modification_response.py
--rw-r--r--   0 root         (0) root         (0)     7998 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/info_response.py
--rw-r--r--   0 root         (0) root         (0)     6618 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_update.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_insert.py
--rw-r--r--   0 root         (0) root         (0)    28275 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6400 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/style_response.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/png_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark.py
--rw-r--r--   0 root         (0) root         (0)    19338 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_text_input.py
--rw-r--r--   0 root         (0) root         (0)     6519 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_response.py
--rw-r--r--   0 root         (0) root         (0)     4792 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/font_dto.py
--rw-r--r--   0 root         (0) root         (0)     7041 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/user_information.py
--rw-r--r--   0 root         (0) root         (0)     7530 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/replace_text_response.py
--rw-r--r--   0 root         (0) root         (0)     9717 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section.py
--rw-r--r--   0 root         (0) root         (0)    19476 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6372 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/runs_response.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_insert_dto.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/run_update.py
--rw-r--r--   0 root         (0) root         (0)     8412 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/time_zone_info_data.py
--rw-r--r--   0 root         (0) root         (0)     7456 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/protection_request.py
--rw-r--r--   0 root         (0) root         (0)    12430 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/metafile_rendering_options_data.py
--rw-r--r--   0 root         (0) root         (0)    10029 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/replace_text_parameters.py
--rw-r--r--   0 root         (0) root         (0)     7710 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/search_response.py
--rw-r--r--   0 root         (0) root         (0)     6607 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/search_results_collection.py
--rw-r--r--   0 root         (0) root         (0)     6668 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_response.py
--rw-r--r--   0 root         (0) root         (0)    16738 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_level_update.py
--rw-r--r--   0 root         (0) root         (0)     6785 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_property_response.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/file_reference.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties_dto.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop_base.py
--rw-r--r--   0 root         (0) root         (0)     7559 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_insert.py
--rw-r--r--   0 root         (0) root         (0)    50559 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/html_fixed_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/replace_range.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/runs.py
--rw-r--r--   0 root         (0) root         (0)     6382 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/files_upload_result.py
--rw-r--r--   0 root         (0) root         (0)    12966 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/outline_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_position.py
--rw-r--r--   0 root         (0) root         (0)    11766 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/border.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/
--rw-r--r--   0 root         (0) root         (0)     7318 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_page_numbers_request.py
--rw-r--r--   0 root         (0) root         (0)     7213 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/append_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5688 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraphs_request.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_request.py
--rw-r--r--   0 root         (0) root         (0)     6203 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     6117 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6286 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     5458 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/build_report_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5415 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5591 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6908 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5111 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmark_by_name_request.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comments_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5332 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     7739 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     4994 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/move_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6866 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_of_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/build_report_request.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5490 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7102 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/split_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7206 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_range_request.py
--rw-r--r--   0 root         (0) root         (0)     7118 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     5625 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8132 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7036 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7473 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_with_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6222 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_statistics_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7179 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6063 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_from_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     6355 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reject_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7627 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5477 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/execute_mail_merge_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6977 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_watermark_request.py
--rw-r--r--   0 root         (0) root         (0)     7849 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     6040 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_request.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/load_web_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5383 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlinks_request.py
--rw-r--r--   0 root         (0) root         (0)     7324 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_request.py
--rw-r--r--   0 root         (0) root         (0)     7750 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_field_request.py
--rw-r--r--   0 root         (0) root         (0)     7780 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_tables_request.py
--rw-r--r--   0 root         (0) root         (0)     4231 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_request.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5654 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_runs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7448 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_image_request.py
--rw-r--r--   0 root         (0) root         (0)     6449 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/protect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6286 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7068 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_list_request.py
--rw-r--r--   0 root         (0) root         (0)     6175 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7816 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5961 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7918 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6076 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6727 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5467 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraphs_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7658 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_image_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7814 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6220 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_with_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
--rw-r--r--   0 root         (0) root         (0)     5909 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7749 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     4223 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_protection_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_lists_request.py
--rw-r--r--   0 root         (0) root         (0)     6856 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8080 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5764 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_field_names_request.py
--rw-r--r--   0 root         (0) root         (0)     7881 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7747 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7128 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_text_request.py
--rw-r--r--   0 root         (0) root         (0)     7996 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8095 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_row_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6462 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/unprotect_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7021 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7607 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_lists_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_macros_request.py
--rw-r--r--   0 root         (0) root         (0)     7943 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7280 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/batch_request.py
--rw-r--r--   0 root         (0) root         (0)     7153 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7260 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_border_request.py
--rw-r--r--   0 root         (0) root         (0)     7124 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_table_request.py
--rw-r--r--   0 root         (0) root         (0)     8072 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_row_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5719 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_field_request.py
--rw-r--r--   0 root         (0) root         (0)     7954 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_border_request.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     8062 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_level_request.py
--rw-r--r--   0 root         (0) root         (0)     6345 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     7109 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6040 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_field_request.py
--rw-r--r--   0 root         (0) root         (0)    10973 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_tiff_request.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/optimize_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7334 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     3361 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_info_request.py
--rw-r--r--   0 root         (0) root         (0)     7711 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7667 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5194 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7168 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_office_math_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_page_request.py
--rw-r--r--   0 root         (0) root         (0)     6250 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_request.py
--rw-r--r--   0 root         (0) root         (0)     6429 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compress_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7091 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_paragraph_request.py
--rw-r--r--   0 root         (0) root         (0)     6392 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compress_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6325 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     5851 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6185 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     4747 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/move_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     5710 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     7910 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6665 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     6410 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     7849 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5711 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_objects_request.py
--rw-r--r--   0 root         (0) root         (0)     5738 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_page_setup_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6910 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     5959 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7519 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_request.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/download_file_request.py
--rw-r--r--   0 root         (0) root         (0)     6244 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_page_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7039 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7052 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7064 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_style_request.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_request.py
--rw-r--r--   0 root         (0) root         (0)     7860 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7029 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7915 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_run_request.py
--rw-r--r--   0 root         (0) root         (0)     6138 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7630 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_bookmark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7724 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compare_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5993 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
--rw-r--r--   0 root         (0) root         (0)     7766 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5732 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tags_request.py
--rw-r--r--   0 root         (0) root         (0)     6984 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/remove_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5641 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnotes_request.py
--rw-r--r--   0 root         (0) root         (0)     6765 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_borders_request.py
--rw-r--r--   0 root         (0) root         (0)     8009 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_list_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7152 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_headers_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/append_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7374 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6208 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7417 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5783 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/accept_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5119 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7200 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)    33549 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6173 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     7082 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     6995 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_properties_request.py
--rw-r--r--   0 root         (0) root         (0)     6240 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_macros_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6659 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5504 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/search_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_text_request.py
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_property_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5948 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmarks_request.py
--rw-r--r--   0 root         (0) root         (0)     7165 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
--rw-r--r--   0 root         (0) root         (0)     6081 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7568 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_style_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7070 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5849 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
--rw-r--r--   0 root         (0) root         (0)    10926 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_tiff_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5498 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7559 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_page_setup_request.py
--rw-r--r--   0 root         (0) root         (0)     7051 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6994 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_styles_from_template_request.py
--rw-r--r--   0 root         (0) root         (0)     6191 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7122 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reset_cache_request.py
--rw-r--r--   0 root         (0) root         (0)     6478 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_range_text_request.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6951 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
--rw-r--r--   0 root         (0) root         (0)     5783 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reject_all_revisions_request.py
--rw-r--r--   0 root         (0) root         (0)     5162 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6839 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/remove_range_request.py
--rw-r--r--   0 root         (0) root         (0)     5511 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7711 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6123 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     7592 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_cell_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_range_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5989 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6910 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_section_request.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_borders_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7149 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_text_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5174 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_protection_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7901 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7784 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_or_update_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     7840 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/apply_style_to_document_element_request.py
--rw-r--r--   0 root         (0) root         (0)     5316 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_styles_request.py
--rw-r--r--   0 root         (0) root         (0)     7094 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_page_numbers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5150 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_sections_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_header_footer_request.py
--rw-r--r--   0 root         (0) root         (0)     5853 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnote_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7946 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_custom_xml_part_request.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_level_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5971 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footers_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     5945 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8351 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5718 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/search_request.py
--rw-r--r--   0 root         (0) root         (0)     7903 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6977 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     8154 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7596 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_comment_request.py
--rw-r--r--   0 root         (0) root         (0)     6637 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_watermark_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6443 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_statistics_request.py
--rw-r--r--   0 root         (0) root         (0)     7011 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/optimize_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7146 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_request.py
--rw-r--r--   0 root         (0) root         (0)     7483 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_parts_request.py
--rw-r--r--   0 root         (0) root         (0)     7112 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_footnote_request.py
--rw-r--r--   0 root         (0) root         (0)     3695 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_available_fonts_request.py
--rw-r--r--   0 root         (0) root         (0)     6917 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_drawing_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7241 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_run_online_request.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/base_request_object.py
--rw-r--r--   0 root         (0) root         (0)     5903 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7005 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_form_field_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_files_list_request.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5750 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_list_request.py
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/split_document_request.py
--rw-r--r--   0 root         (0) root         (0)     7136 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5552 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_field_names_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7707 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7666 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     5854 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5921 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_properties_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7653 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_structured_document_tag_request.py
--rw-r--r--   0 root         (0) root         (0)     6610 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/convert_document_request.py
--rw-r--r--   0 root         (0) root         (0)     6118 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compare_document_request.py
--rw-r--r--   0 root         (0) root         (0)     5779 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6415 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6793 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7001 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5095 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_styles_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5862 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_request.py
--rw-r--r--   0 root         (0) root         (0)     6080 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_field_request.py
--rw-r--r--   0 root         (0) root         (0)     8051 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_font_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5957 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7269 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_headers_footers_request.py
--rw-r--r--   0 root         (0) root         (0)     7098 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_style_request.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_format_request.py
--rw-r--r--   0 root         (0) root         (0)     6397 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/protect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5652 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6079 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7390 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_cell_request.py
--rw-r--r--   0 root         (0) root         (0)     5537 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_list_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmark_request.py
--rw-r--r--   0 root         (0) root         (0)     7555 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/execute_mail_merge_request.py
--rw-r--r--   0 root         (0) root         (0)     5617 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_fields_request.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_runs_request.py
--rw-r--r--   0 root         (0) root         (0)     8359 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_drawing_object_request.py
--rw-r--r--   0 root         (0) root         (0)     7412 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_border_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6374 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comments_request.py
--rw-r--r--   0 root         (0) root         (0)     5933 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_object_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6255 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmarks_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6159 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
--rw-r--r--   0 root         (0) root         (0)     7161 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_range_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5165 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6969 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_document_property_request.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_comment_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6416 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/unprotect_document_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6171 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_paragraph_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7977 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_request.py
--rw-r--r--   0 root         (0) root         (0)     4877 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/upload_file_request.py
--rw-r--r--   0 root         (0) root         (0)     8075 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_font_request.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_public_key_request.py
--rw-r--r--   0 root         (0) root         (0)     6036 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)     6541 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_fields_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5435 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_tables_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7557 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_row_request.py
--rw-r--r--   0 root         (0) root         (0)     5916 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/accept_all_revisions_online_request.py
--rw-r--r--   0 root         (0) root         (0)     4219 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_file_request.py
--rw-r--r--   0 root         (0) root         (0)     5420 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnotes_online_request.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_sections_request.py
--rw-r--r--   0 root         (0) root         (0)     7506 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_with_text_request.py
--rw-r--r--   0 root         (0) root         (0)     6791 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_section_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7308 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
--rw-r--r--   0 root         (0) root         (0)     7284 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_header_footer_online_request.py
--rw-r--r--   0 root         (0) root         (0)    29269 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_properties.py
--rw-r--r--   0 root         (0) root         (0)     6671 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_format_update.py
--rw-r--r--   0 root         (0) root         (0)     5744 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_property_create_or_update.py
--rw-r--r--   0 root         (0) root         (0)    25901 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_flow_pack_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    45532 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/emf_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    43767 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_base.py
--rw-r--r--   0 root         (0) root         (0)     9470 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/shading.py
--rw-r--r--   0 root         (0) root         (0)     9094 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/words_api_link.py
--rw-r--r--   0 root         (0) root         (0)    43991 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_update.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/public_key_response.py
--rw-r--r--   0 root         (0) root         (0)     7603 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/error.py
--rw-r--r--   0 root         (0) root         (0)     8044 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_insert.py
--rw-r--r--   0 root         (0) root         (0)     6617 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_names_response.py
--rw-r--r--   0 root         (0) root         (0)     6774 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_link.py
--rw-r--r--   0 root         (0) root         (0)    28052 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/docx_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9741 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comment_update.py
--rw-r--r--   0 root         (0) root         (0)     7475 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/stat_data_response.py
--rw-r--r--   0 root         (0) root         (0)     6881 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/run_link.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_fields_response.py
--rw-r--r--   0 root         (0) root         (0)    45246 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks.py
--rw-r--r--   0 root         (0) root         (0)     6332 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/lists.py
--rw-r--r--   0 root         (0) root         (0)     8308 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/list_format.py
--rw-r--r--   0 root         (0) root         (0)     6992 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_response.py
--rw-r--r--   0 root         (0) root         (0)     8924 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_insert.py
--rw-r--r--   0 root         (0) root         (0)     6344 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_response.py
--rw-r--r--   0 root         (0) root         (0)     6527 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6939 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part.py
--rw-r--r--   0 root         (0) root         (0)    34298 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/pcl_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6403 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_insert.py
--rw-r--r--   0 root         (0) root         (0)     6884 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/preferred_width.py
--rw-r--r--   0 root         (0) root         (0)     6484 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/error_details.py
--rw-r--r--   0 root         (0) root         (0)    33416 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/text_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)    48113 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/font.py
--rw-r--r--   0 root         (0) root         (0)     6382 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/border_response.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     5788 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_insert.py
--rw-r--r--   0 root         (0) root         (0)     6869 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_list_item.py
--rw-r--r--   0 root         (0) root         (0)     8182 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/font_info.py
--rw-r--r--   0 root         (0) root         (0)     6317 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_names.py
--rw-r--r--   0 root         (0) root         (0)     6694 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section_link_collection.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_link.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/link.py
--rw-r--r--   0 root         (0) root         (0)     7024 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_insert.py
--rw-r--r--   0 root         (0) root         (0)     6675 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format_response.py
--rw-r--r--   0 root         (0) root         (0)     8461 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/storage_file.py
--rw-r--r--   0 root         (0) root         (0)     6712 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnotes_stat_data.py
--rw-r--r--   0 root         (0) root         (0)     8043 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row.py
--rw-r--r--   0 root         (0) root         (0)    19951 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/field_options.py
--rw-r--r--   0 root         (0) root         (0)    27751 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/doc_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlink.py
--rw-r--r--   0 root         (0) root         (0)     5322 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_permissions.py
--rw-r--r--   0 root         (0) root         (0)     6362 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_response.py
--rw-r--r--   0 root         (0) root         (0)     9736 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/page_number.py
--rw-r--r--   0 root         (0) root         (0)     5581 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/files_list.py
--rw-r--r--   0 root         (0) root         (0)     6420 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section_response.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/api_error.py
--rw-r--r--   0 root         (0) root         (0)     6595 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties_response.py
--rw-r--r--   0 root         (0) root         (0)     8974 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/available_fonts_response.py
--rw-r--r--   0 root         (0) root         (0)     4834 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format_dto.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/search_result.py
--rw-r--r--   0 root         (0) root         (0)     8534 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/page_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    25627 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_flow_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     9840 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/json_data_load_options.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/section_link.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/compress_options.py
--rw-r--r--   0 root         (0) root         (0)    76949 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/mhtml_save_options_data.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/run.py
--rw-r--r--   0 root         (0) root         (0)     5648 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/words_response.py
--rw-r--r--   0 root         (0) root         (0)    11010 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/footnote.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/link_element.py
--rw-r--r--   0 root         (0) root         (0)     7902 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_encryption_details_data.py
--rw-r--r--   0 root         (0) root         (0)     9741 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/comment_insert.py
--rw-r--r--   0 root         (0) root         (0)     6322 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_link.py
--rw-r--r--   0 root         (0) root         (0)     8156 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_entry_list.py
--rw-r--r--   0 root         (0) root         (0)    14358 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/form_field.py
--rw-r--r--   0 root         (0) root         (0)     9637 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/models/document_stat_data.py
--rw-r--r--   0 root         (0) root         (0)    11506 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/rest.py
--rw-r--r--   0 root         (0) root         (0)    19684 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9423 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/asposewordscloud/apis/
--rw-r--r--   0 root         (0) root         (0)  1380535 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/apis/words_api.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30710 2023-06-29 06:02:49.000000 aspose-words-cloud-23.5.1/asposewordscloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    39456 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    13759 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 06:03:26.000000 aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 06:03:27.000000 aspose-words-cloud-23.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-14 07:45:24.000000 aspose-words-cloud-23.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12600 2023-07-14 07:45:24.000000 aspose-words-cloud-23.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/test/
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/base_test_context.py
+-rw-r--r--   0 root         (0) root         (0)     9634 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_examples.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_url_encode.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_doc_with_password.py
+-rw-r--r--   0 root         (0) root         (0)     4054 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/test/test_readme.py
+-rw-r--r--   0 root         (0) root         (0)    13836 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/
+-rw-r--r--   0 root         (0) root         (0)    11024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_apply.py
+-rw-r--r--   0 root         (0) root         (0)    45668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/jpeg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_response.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6354 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_response.py
+-rw-r--r--   0 root         (0) root         (0)     8614 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/csv_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bmp_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    24397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/word_ml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_response.py
+-rw-r--r--   0 root         (0) root         (0)     6444 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_levels.py
+-rw-r--r--   0 root         (0) root         (0)     6538 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_response.py
+-rw-r--r--   0 root         (0) root         (0)     6915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)     6467 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/lists_response.py
+-rw-r--r--   0 root         (0) root         (0)    14309 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6411 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object_response.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/fields_response.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    27747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dot_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry.py
+-rw-r--r--   0 root         (0) root         (0)    23377 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style.py
+-rw-r--r--   0 root         (0) root         (0)     7026 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_link.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dotx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    50657 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tiff_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/save_response.py
+-rw-r--r--   0 root         (0) root         (0)     6292 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_response.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_response.py
+-rw-r--r--   0 root         (0) root         (0)    76376 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/epub_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_list_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/new_document_position.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xml_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_update.py
+-rw-r--r--   0 root         (0) root         (0)    28013 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/ott_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell.py
+-rw-r--r--   0 root         (0) root         (0)     6550 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6767 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks_response.py
+-rw-r--r--   0 root         (0) root         (0)     6779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_outline_level_data.py
+-rw-r--r--   0 root         (0) root         (0)    13381 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_update.py
+-rw-r--r--   0 root         (0) root         (0)    34808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_update.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph.py
+-rw-r--r--   0 root         (0) root         (0)     6565 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_response.py
+-rw-r--r--   0 root         (0) root         (0)     7537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_result.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format.py
+-rw-r--r--   0 root         (0) root         (0)     7099 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tags_response.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_page_setup_response.py
+-rw-r--r--   0 root         (0) root         (0)     6496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink_response.py
+-rw-r--r--   0 root         (0) root         (0)     8434 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field.py
+-rw-r--r--   0 root         (0) root         (0)     9407 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer.py
+-rw-r--r--   0 root         (0) root         (0)     6524 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stops_response.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_response.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_response.py
+-rw-r--r--   0 root         (0) root         (0)    40523 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_setup.py
+-rw-r--r--   0 root         (0) root         (0)    28040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_data.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_response.py
+-rw-r--r--   0 root         (0) root         (0)    30577 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/markdown_save_options_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_header_footer_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compress_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compare_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/protect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_font_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_fields_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_with_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_row_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_row_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_borders_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/remove_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_bookmark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_footnote_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     7176 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_comment_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_tiff_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/unprotect_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_form_field_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_border_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_range_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_properties_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/split_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_paragraph_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/copy_style_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_level_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_watermark_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_cell_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_drawing_object_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/append_document_online_response.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/docm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    32952 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/ps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6525 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comments_collection.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/dotm_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_response.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop.py
+-rw-r--r--   0 root         (0) root         (0)     6621 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link.py
+-rw-r--r--   0 root         (0) root         (0)     6248 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xml_color.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_update.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_response.py
+-rw-r--r--   0 root         (0) root         (0)    34159 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_response.py
+-rw-r--r--   0 root         (0) root         (0)     6496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_response.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7608 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5761 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_response.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_link.py
+-rw-r--r--   0 root         (0) root         (0)     8999 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/file_link.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/node_link.py
+-rw-r--r--   0 root         (0) root         (0)     7697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data_response.py
+-rw-r--r--   0 root         (0) root         (0)    34808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_insert.py
+-rw-r--r--   0 root         (0) root         (0)    16483 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compare_options.py
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/load_web_document_data.py
+-rw-r--r--   0 root         (0) root         (0)     8854 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_update.py
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/report_build_options.py
+-rw-r--r--   0 root         (0) root         (0)     6388 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_text_response.py
+-rw-r--r--   0 root         (0) root         (0)     6773 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)    11839 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/report_engine_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6464 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     6389 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_collection.py
+-rw-r--r--   0 root         (0) root         (0)     7072 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_insert.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_link.py
+-rw-r--r--   0 root         (0) root         (0)     8058 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/modification_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     6810 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_collection.py
+-rw-r--r--   0 root         (0) root         (0)    17850 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection_response.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/range_document.py
+-rw-r--r--   0 root         (0) root         (0)     5739 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/story_child_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link.py
+-rw-r--r--   0 root         (0) root         (0)     6691 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_response.py
+-rw-r--r--   0 root         (0) root         (0)     6366 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_link.py
+-rw-r--r--   0 root         (0) root         (0)     8453 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/downsample_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10167 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_digital_signature_details_data.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format.py
+-rw-r--r--   0 root         (0) root         (0)     7673 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/save_result.py
+-rw-r--r--   0 root         (0) root         (0)     8245 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_insert.py
+-rw-r--r--   0 root         (0) root         (0)    36909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/open_xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/optimization_options.py
+-rw-r--r--   0 root         (0) root         (0)     6788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range_dto.py
+-rw-r--r--   0 root         (0) root         (0)    12026 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/styles_response.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data.py
+-rw-r--r--   0 root         (0) root         (0)    28658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     5915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry.py
+-rw-r--r--   0 root         (0) root         (0)    11051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compress_response.py
+-rw-r--r--   0 root         (0) root         (0)    28017 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/odt_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_update.py
+-rw-r--r--   0 root         (0) root         (0)    16964 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_drop_down.py
+-rw-r--r--   0 root         (0) root         (0)    12508 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_info.py
+-rw-r--r--   0 root         (0) root         (0)     8786 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/classification_response.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     9566 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compare_data.py
+-rw-r--r--   0 root         (0) root         (0)    28036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/rtf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/watermark_text.py
+-rw-r--r--   0 root         (0) root         (0)     8079 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/info_additional_item.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/borders_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6335 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/classification_result.py
+-rw-r--r--   0 root         (0) root         (0)    75129 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/html_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    34704 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6770 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comments_response.py
+-rw-r--r--   0 root         (0) root         (0)    38869 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/svg_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    28886 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/gif_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6492 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/borders_response.py
+-rw-r--r--   0 root         (0) root         (0)     6773 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footers_response.py
+-rw-r--r--   0 root         (0) root         (0)    36496 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xps_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    18821 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_level.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_insert.py
+-rw-r--r--   0 root         (0) root         (0)    67826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     5704 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_copy.py
+-rw-r--r--   0 root         (0) root         (0)    17661 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object.py
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/revisions_modification_response.py
+-rw-r--r--   0 root         (0) root         (0)     7998 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/info_response.py
+-rw-r--r--   0 root         (0) root         (0)     6618 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_update.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_insert.py
+-rw-r--r--   0 root         (0) root         (0)    28275 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6400 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/style_response.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/png_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark.py
+-rw-r--r--   0 root         (0) root         (0)    19338 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_text_input.py
+-rw-r--r--   0 root         (0) root         (0)     6519 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_response.py
+-rw-r--r--   0 root         (0) root         (0)     4792 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/user_information.py
+-rw-r--r--   0 root         (0) root         (0)     7530 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_response.py
+-rw-r--r--   0 root         (0) root         (0)     9717 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section.py
+-rw-r--r--   0 root         (0) root         (0)    19476 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6372 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/runs_response.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_update.py
+-rw-r--r--   0 root         (0) root         (0)     8412 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/time_zone_info_data.py
+-rw-r--r--   0 root         (0) root         (0)     7456 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/protection_request.py
+-rw-r--r--   0 root         (0) root         (0)    12430 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/metafile_rendering_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     7710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_response.py
+-rw-r--r--   0 root         (0) root         (0)     6607 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_results_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_response.py
+-rw-r--r--   0 root         (0) root         (0)    16738 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_level_update.py
+-rw-r--r--   0 root         (0) root         (0)     6785 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_response.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/file_reference.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_dto.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_base.py
+-rw-r--r--   0 root         (0) root         (0)     7559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert.py
+-rw-r--r--   0 root         (0) root         (0)    50559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/html_fixed_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range.py
+-rw-r--r--   0 root         (0) root         (0)     6190 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/runs.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/files_upload_result.py
+-rw-r--r--   0 root         (0) root         (0)    12966 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/outline_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_position.py
+-rw-r--r--   0 root         (0) root         (0)    11766 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/border.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/
+-rw-r--r--   0 root         (0) root         (0)     7318 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7213 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_request.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     6117 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     5458 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5591 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6908 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5332 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     7739 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6866 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6917 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_request.py
+-rw-r--r--   0 root         (0) root         (0)     4977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7206 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     7118 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     5625 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7473 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7179 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6063 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     6355 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7627 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/load_web_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     7780 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5656 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_request.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_request.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5654 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_request.py
+-rw-r--r--   0 root         (0) root         (0)     6449 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7068 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     6175 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7816 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7918 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6727 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5467 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7658 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7814 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_with_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py
+-rw-r--r--   0 root         (0) root         (0)     5909 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7749 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_request.py
+-rw-r--r--   0 root         (0) root         (0)     6856 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8080 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_request.py
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     7996 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8095 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6462 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7021 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7607 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5087 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_request.py
+-rw-r--r--   0 root         (0) root         (0)     7943 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/batch_request.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7260 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     7124 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_request.py
+-rw-r--r--   0 root         (0) root         (0)     8072 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5719 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     7954 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_request.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     8062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_request.py
+-rw-r--r--   0 root         (0) root         (0)     6345 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     7109 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_request.py
+-rw-r--r--   0 root         (0) root         (0)    10973 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_request.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     3361 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_info_request.py
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7168 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_request.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_request.py
+-rw-r--r--   0 root         (0) root         (0)     6429 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7091 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_request.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6325 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     5851 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6185 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     4747 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     7910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6665 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_request.py
+-rw-r--r--   0 root         (0) root         (0)     5738 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     5959 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7519 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/download_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     6244 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7039 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7064 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     7860 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7029 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7915 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     6138 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7724 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5732 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_request.py
+-rw-r--r--   0 root         (0) root         (0)     6984 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_request.py
+-rw-r--r--   0 root         (0) root         (0)     6765 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_request.py
+-rw-r--r--   0 root         (0) root         (0)     8009 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7152 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7374 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6208 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7417 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7200 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)    33549 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_request.py
+-rw-r--r--   0 root         (0) root         (0)     6240 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6659 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5948 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_request.py
+-rw-r--r--   0 root         (0) root         (0)     7165 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py
+-rw-r--r--   0 root         (0) root         (0)     6081 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7568 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5849 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    10926 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5498 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7559 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_request.py
+-rw-r--r--   0 root         (0) root         (0)     7051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6994 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_styles_from_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reset_cache_request.py
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6951 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_request.py
+-rw-r--r--   0 root         (0) root         (0)     5162 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6839 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_request.py
+-rw-r--r--   0 root         (0) root         (0)     5511 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7711 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7521 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     7592 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6264 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6910 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7149 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5174 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7901 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     7840 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py
+-rw-r--r--   0 root         (0) root         (0)     5316 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_request.py
+-rw-r--r--   0 root         (0) root         (0)     7094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_request.py
+-rw-r--r--   0 root         (0) root         (0)     5853 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5695 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7946 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_request.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     5945 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8351 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5718 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     7903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     8154 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7596 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_request.py
+-rw-r--r--   0 root         (0) root         (0)     6637 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6443 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_request.py
+-rw-r--r--   0 root         (0) root         (0)     7011 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7146 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     7483 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_request.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_available_fonts_request.py
+-rw-r--r--   0 root         (0) root         (0)     6917 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7241 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_online_request.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/base_request_object.py
+-rw-r--r--   0 root         (0) root         (0)     5903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7005 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_files_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5750 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_request.py
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     7136 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7707 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7666 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     5854 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     6610 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/convert_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     6118 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     5779 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6415 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6793 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7001 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5862 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_request.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_request.py
+-rw-r--r--   0 root         (0) root         (0)     8051 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5957 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_request.py
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_request.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_request.py
+-rw-r--r--   0 root         (0) root         (0)     6397 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7390 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_request.py
+-rw-r--r--   0 root         (0) root         (0)     5537 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_request.py
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_request.py
+-rw-r--r--   0 root         (0) root         (0)     5617 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_request.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_request.py
+-rw-r--r--   0 root         (0) root         (0)     8359 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     7412 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6374 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_request.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6159 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     7161 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5165 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6969 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_request.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6171 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7977 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/upload_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     8075 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_request.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_public_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     6541 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5435 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7557 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_request.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_file_request.py
+-rw-r--r--   0 root         (0) root         (0)     5420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_request.py
+-rw-r--r--   0 root         (0) root         (0)     7506 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_request.py
+-rw-r--r--   0 root         (0) root         (0)     6791 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_online_request.py
+-rw-r--r--   0 root         (0) root         (0)    29269 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     5744 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_create_or_update.py
+-rw-r--r--   0 root         (0) root         (0)    25901 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    45532 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/emf_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    43767 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_base.py
+-rw-r--r--   0 root         (0) root         (0)     9470 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/shading.py
+-rw-r--r--   0 root         (0) root         (0)     9094 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_link.py
+-rw-r--r--   0 root         (0) root         (0)    43991 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_update.py
+-rw-r--r--   0 root         (0) root         (0)     7296 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/public_key_response.py
+-rw-r--r--   0 root         (0) root         (0)     7603 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     8044 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_names_response.py
+-rw-r--r--   0 root         (0) root         (0)     6774 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link.py
+-rw-r--r--   0 root         (0) root         (0)    28052 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/docx_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_update.py
+-rw-r--r--   0 root         (0) root         (0)     7475 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/stat_data_response.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run_link.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_fields_response.py
+-rw-r--r--   0 root         (0) root         (0)    45246 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format.py
+-rw-r--r--   0 root         (0) root         (0)     6437 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks.py
+-rw-r--r--   0 root         (0) root         (0)     6332 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/lists.py
+-rw-r--r--   0 root         (0) root         (0)     8308 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/list_format.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_response.py
+-rw-r--r--   0 root         (0) root         (0)     8924 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6344 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_response.py
+-rw-r--r--   0 root         (0) root         (0)     6527 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6939 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part.py
+-rw-r--r--   0 root         (0) root         (0)    34298 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pcl_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6403 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6884 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/preferred_width.py
+-rw-r--r--   0 root         (0) root         (0)     6484 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/error_details.py
+-rw-r--r--   0 root         (0) root         (0)    33416 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/text_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)    48113 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/border_response.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     5788 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6869 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_list_item.py
+-rw-r--r--   0 root         (0) root         (0)     8182 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/font_info.py
+-rw-r--r--   0 root         (0) root         (0)     6317 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_names.py
+-rw-r--r--   0 root         (0) root         (0)     6694 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_link.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_response.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/storage_file.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)     8043 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row.py
+-rw-r--r--   0 root         (0) root         (0)    19951 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/field_options.py
+-rw-r--r--   0 root         (0) root         (0)    27751 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/doc_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     6362 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_response.py
+-rw-r--r--   0 root         (0) root         (0)     9736 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_number.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/files_list.py
+-rw-r--r--   0 root         (0) root         (0)     6420 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_response.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     6595 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_response.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/available_fonts_response.py
+-rw-r--r--   0 root         (0) root         (0)     4834 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/search_result.py
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/page_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    25627 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     9840 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/json_data_load_options.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/section_link.py
+-rw-r--r--   0 root         (0) root         (0)     7375 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/compress_options.py
+-rw-r--r--   0 root         (0) root         (0)    76949 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/mhtml_save_options_data.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/run.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/words_response.py
+-rw-r--r--   0 root         (0) root         (0)    11010 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/footnote.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/link_element.py
+-rw-r--r--   0 root         (0) root         (0)     7902 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_encryption_details_data.py
+-rw-r--r--   0 root         (0) root         (0)     9741 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/comment_insert.py
+-rw-r--r--   0 root         (0) root         (0)     6322 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_link.py
+-rw-r--r--   0 root         (0) root         (0)     8156 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry_list.py
+-rw-r--r--   0 root         (0) root         (0)    14358 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/form_field.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/models/document_stat_data.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/rest.py
+-rw-r--r--   0 root         (0) root         (0)    19684 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/
+-rw-r--r--   0 root         (0) root         (0)  1380535 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/words_api.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30710 2023-07-14 07:45:25.000000 aspose-words-cloud-23.6.0/asposewordscloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    39456 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    13836 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 07:46:02.000000 aspose-words-cloud-23.6.0/setup.cfg
```

### Comparing `aspose-words-cloud-23.5.1/LICENSE` & `aspose-words-cloud-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/README.md` & `aspose-words-cloud-23.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 23.6
+
+- Fix XMLHttpRequest in web applications.
+
+
 ## Enhancements in Version 23.5
 
 - Added InsertSection method.
 
 
 ## Enhancements in Version 23.4
```

### Comparing `aspose-words-cloud-23.5.1/test/base_test_context.py` & `aspose-words-cloud-23.6.0/test/base_test_context.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/test_batch.py` & `aspose-words-cloud-23.6.0/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/test_examples.py` & `aspose-words-cloud-23.6.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/__init__.py` & `aspose-words-cloud-23.6.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/test_url_encode.py` & `aspose-words-cloud-23.6.0/test/test_url_encode.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/test_doc_with_password.py` & `aspose-words-cloud-23.6.0/test/test_doc_with_password.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/test/test_readme.py` & `aspose-words-cloud-23.6.0/test/test_readme.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/PKG-INFO` & `aspose-words-cloud-23.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 23.5.1
+Version: 23.6.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
@@ -34,14 +34,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 23.6
+
+- Fix XMLHttpRequest in web applications.
+
+
 ## Enhancements in Version 23.5
 
 - Added InsertSection method.
 
 
 ## Enhancements in Version 23.4
```

### Comparing `aspose-words-cloud-23.5.1/setup.py` & `aspose-words-cloud-23.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     Aspose.Words for Cloud API Reference
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 23.5
+    OpenAPI spec version: 23.6
 
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "aspose-words-cloud"
-VERSION = "23.5.1"
+VERSION = "23.6.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,56 +38,78 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'links': 'list[Link]',
         'document_properties': 'DocumentProperties',
         'file_name': 'str',
         'is_encrypted': 'bool',
         'is_signed': 'bool',
-        'links': 'list[Link]',
         'source_format': 'str'
     }
 
     attribute_map = {
+        'links': 'Links',
         'document_properties': 'DocumentProperties',
         'file_name': 'FileName',
         'is_encrypted': 'IsEncrypted',
         'is_signed': 'IsSigned',
-        'links': 'Links',
         'source_format': 'SourceFormat'
     }
 
-    def __init__(self, document_properties=None, file_name=None, is_encrypted=None, is_signed=None, links=None, source_format=None):  # noqa: E501
+    def __init__(self, links=None, document_properties=None, file_name=None, is_encrypted=None, is_signed=None, source_format=None):  # noqa: E501
         """Document - a model defined in Swagger"""  # noqa: E501
 
+        self._links = None
         self._document_properties = None
         self._file_name = None
         self._is_encrypted = None
         self._is_signed = None
-        self._links = None
         self._source_format = None
         self.discriminator = None
 
+        if links is not None:
+            self.links = links
         if document_properties is not None:
             self.document_properties = document_properties
         if file_name is not None:
             self.file_name = file_name
         if is_encrypted is not None:
             self.is_encrypted = is_encrypted
         if is_signed is not None:
             self.is_signed = is_signed
-        if links is not None:
-            self.links = links
         if source_format is not None:
             self.source_format = source_format
 
     @property
+    def links(self):
+        """Gets the links of this Document.  # noqa: E501
+
+        Gets or sets the list of links that originate from this document.  # noqa: E501
+
+        :return: The links of this Document.  # noqa: E501
+        :rtype: list[Link]
+        """
+        return self._links
+
+    @links.setter
+    def links(self, links):
+        """Sets the links of this Document.
+
+        Gets or sets the list of links that originate from this document.  # noqa: E501
+
+        :param links: The links of this Document.  # noqa: E501
+        :type: list[Link]
+        """
+        self._links = links
+
+    @property
     def document_properties(self):
         """Gets the document_properties of this Document.  # noqa: E501
 
         Gets or sets the document properties.  # noqa: E501
 
         :return: The document_properties of this Document.  # noqa: E501
         :rtype: DocumentProperties
@@ -168,36 +190,14 @@
 
         :param is_signed: The is_signed of this Document.  # noqa: E501
         :type: bool
         """
         self._is_signed = is_signed
 
     @property
-    def links(self):
-        """Gets the links of this Document.  # noqa: E501
-
-        Gets or sets the list of links that originate from this document.  # noqa: E501
-
-        :return: The links of this Document.  # noqa: E501
-        :rtype: list[Link]
-        """
-        return self._links
-
-    @links.setter
-    def links(self, links):
-        """Sets the links of this Document.
-
-        Gets or sets the list of links that originate from this document.  # noqa: E501
-
-        :param links: The links of this Document.  # noqa: E501
-        :type: list[Link]
-        """
-        self._links = links
-
-    @property
     def source_format(self):
         """Gets the source_format of this Document.  # noqa: E501
 
         Gets or sets the original format of the document.  # noqa: E501
 
         :return: The source_format of this Document.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style_apply.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style_apply.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/jpeg_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/jpeg_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
+        'use_gdi_emf_renderer': 'bool',
         'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
@@ -103,21 +103,21 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None):  # noqa: E501
         """JpegSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -141,17 +141,17 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
+        self._use_gdi_emf_renderer = None
         self._save_format = "jpeg"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
@@ -205,20 +205,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def allow_embedding_post_script_fonts(self):
         """Gets the allow_embedding_post_script_fonts of this JpegSaveOptionsData.  # noqa: E501
 
         Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false..  # noqa: E501
 
@@ -915,36 +915,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this JpegSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this JpegSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this JpegSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this JpegSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -981,14 +959,36 @@
 
         :param vertical_resolution: The vertical_resolution of this JpegSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :return: The use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this JpegSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this JpegSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
+
+    @property
     def save_format(self):
         """Gets the save_format of this JpegSaveOptionsData.  # noqa: E501
 
         Gets the format of save.  # noqa: E501
 
         :return: The save_format of this JpegSaveOptionsData.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_parts_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/csv_data_load_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/csv_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bmp_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bmp_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
+        'use_gdi_emf_renderer': 'bool',
         'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
@@ -103,21 +103,21 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None):  # noqa: E501
         """BmpSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -141,17 +141,17 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
+        self._use_gdi_emf_renderer = None
         self._save_format = "bmp"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
@@ -205,20 +205,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def allow_embedding_post_script_fonts(self):
         """Gets the allow_embedding_post_script_fonts of this BmpSaveOptionsData.  # noqa: E501
 
         Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false..  # noqa: E501
 
@@ -915,36 +915,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this BmpSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this BmpSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this BmpSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this BmpSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -981,14 +959,36 @@
 
         :param vertical_resolution: The vertical_resolution of this BmpSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :return: The use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this BmpSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this BmpSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
+
+    @property
     def save_format(self):
         """Gets the save_format of this BmpSaveOptionsData.  # noqa: E501
 
         Gets the format of save.  # noqa: E501
 
         :return: The save_format of this BmpSaveOptionsData.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/word_ml_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/word_ml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_levels.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_levels.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_objects_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/lists_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/lists_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_object_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/fields_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/image_entry_list.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/dot_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/dot_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_entry.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,23 @@
         """Sets the import_format_mode of this DocumentEntry.
 
         Gets or sets the option that controls formatting will be used: appended or destination document. Can be KeepSourceFormatting or UseDestinationStyles.  # noqa: E501
 
         :param import_format_mode: The import_format_mode of this DocumentEntry.  # noqa: E501
         :type: str
         """
-        self._import_format_mode = import_format_mode
+        allowed_values = ["UseDestinationStyles", "KeepSourceFormatting", "KeepDifferentStyles"]  # noqa: E501
+        if not import_format_mode.isdigit():
+            if import_format_mode not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `import_format_mode` ({0}), must be one of {1}"  # noqa: E501
+                    .format(import_format_mode, allowed_values))
+            self._import_format_mode = import_format_mode
+        else:
+            self._import_format_mode = allowed_values[int(import_format_mode) if six.PY3 else long(import_format_mode)]
 
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
         if self._file_reference is not None:
             self._file_reference.extract_files_content(filesContentResult)
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,83 +39,83 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'aliases': 'list[str]',
-        'base_style_name': 'str',
-        'built_in': 'bool',
         'font': 'Font',
-        'is_heading': 'bool',
+        'built_in': 'bool',
+        'next_paragraph_style_name': 'str',
+        'base_style_name': 'str',
         'is_quick_style': 'bool',
         'linked_style_name': 'str',
-        'name': 'str',
-        'next_paragraph_style_name': 'str',
+        'type': 'str',
+        'is_heading': 'bool',
+        'aliases': 'list[str]',
         'style_identifier': 'str',
-        'type': 'str'
+        'name': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
-        'aliases': 'Aliases',
-        'base_style_name': 'BaseStyleName',
-        'built_in': 'BuiltIn',
         'font': 'Font',
-        'is_heading': 'IsHeading',
+        'built_in': 'BuiltIn',
+        'next_paragraph_style_name': 'NextParagraphStyleName',
+        'base_style_name': 'BaseStyleName',
         'is_quick_style': 'IsQuickStyle',
         'linked_style_name': 'LinkedStyleName',
-        'name': 'Name',
-        'next_paragraph_style_name': 'NextParagraphStyleName',
+        'type': 'Type',
+        'is_heading': 'IsHeading',
+        'aliases': 'Aliases',
         'style_identifier': 'StyleIdentifier',
-        'type': 'Type'
+        'name': 'Name'
     }
 
-    def __init__(self, link=None, aliases=None, base_style_name=None, built_in=None, font=None, is_heading=None, is_quick_style=None, linked_style_name=None, name=None, next_paragraph_style_name=None, style_identifier=None, type=None):  # noqa: E501
+    def __init__(self, link=None, font=None, built_in=None, next_paragraph_style_name=None, base_style_name=None, is_quick_style=None, linked_style_name=None, type=None, is_heading=None, aliases=None, style_identifier=None, name=None):  # noqa: E501
         """Style - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._aliases = None
-        self._base_style_name = None
-        self._built_in = None
         self._font = None
-        self._is_heading = None
+        self._built_in = None
+        self._next_paragraph_style_name = None
+        self._base_style_name = None
         self._is_quick_style = None
         self._linked_style_name = None
-        self._name = None
-        self._next_paragraph_style_name = None
-        self._style_identifier = None
         self._type = None
+        self._is_heading = None
+        self._aliases = None
+        self._style_identifier = None
+        self._name = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if aliases is not None:
-            self.aliases = aliases
-        if base_style_name is not None:
-            self.base_style_name = base_style_name
-        if built_in is not None:
-            self.built_in = built_in
         if font is not None:
             self.font = font
-        if is_heading is not None:
-            self.is_heading = is_heading
+        if built_in is not None:
+            self.built_in = built_in
+        if next_paragraph_style_name is not None:
+            self.next_paragraph_style_name = next_paragraph_style_name
+        if base_style_name is not None:
+            self.base_style_name = base_style_name
         if is_quick_style is not None:
             self.is_quick_style = is_quick_style
         if linked_style_name is not None:
             self.linked_style_name = linked_style_name
-        if name is not None:
-            self.name = name
-        if next_paragraph_style_name is not None:
-            self.next_paragraph_style_name = next_paragraph_style_name
-        if style_identifier is not None:
-            self.style_identifier = style_identifier
         if type is not None:
             self.type = type
+        if is_heading is not None:
+            self.is_heading = is_heading
+        if aliases is not None:
+            self.aliases = aliases
+        if style_identifier is not None:
+            self.style_identifier = style_identifier
+        if name is not None:
+            self.name = name
 
     @property
     def link(self):
         """Gets the link of this Style.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -132,56 +132,34 @@
 
         :param link: The link of this Style.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def aliases(self):
-        """Gets the aliases of this Style.  # noqa: E501
-
-        Gets or sets all aliases of this style. If style has no aliases then empty array of string is returned.  # noqa: E501
-
-        :return: The aliases of this Style.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._aliases
-
-    @aliases.setter
-    def aliases(self, aliases):
-        """Sets the aliases of this Style.
-
-        Gets or sets all aliases of this style. If style has no aliases then empty array of string is returned.  # noqa: E501
-
-        :param aliases: The aliases of this Style.  # noqa: E501
-        :type: list[str]
-        """
-        self._aliases = aliases
-
-    @property
-    def base_style_name(self):
-        """Gets the base_style_name of this Style.  # noqa: E501
+    def font(self):
+        """Gets the font of this Style.  # noqa: E501
 
-        Gets or sets the name of the style this style is based on.  # noqa: E501
+        Gets or sets the character formatting of the style.  # noqa: E501
 
-        :return: The base_style_name of this Style.  # noqa: E501
-        :rtype: str
+        :return: The font of this Style.  # noqa: E501
+        :rtype: Font
         """
-        return self._base_style_name
+        return self._font
 
-    @base_style_name.setter
-    def base_style_name(self, base_style_name):
-        """Sets the base_style_name of this Style.
+    @font.setter
+    def font(self, font):
+        """Sets the font of this Style.
 
-        Gets or sets the name of the style this style is based on.  # noqa: E501
+        Gets or sets the character formatting of the style.  # noqa: E501
 
-        :param base_style_name: The base_style_name of this Style.  # noqa: E501
-        :type: str
+        :param font: The font of this Style.  # noqa: E501
+        :type: Font
         """
-        self._base_style_name = base_style_name
+        self._font = font
 
     @property
     def built_in(self):
         """Gets the built_in of this Style.  # noqa: E501
 
         Gets or sets a value indicating whether this style is one of the built-in styles in MS Word.  # noqa: E501
 
@@ -198,56 +176,56 @@
 
         :param built_in: The built_in of this Style.  # noqa: E501
         :type: bool
         """
         self._built_in = built_in
 
     @property
-    def font(self):
-        """Gets the font of this Style.  # noqa: E501
+    def next_paragraph_style_name(self):
+        """Gets the next_paragraph_style_name of this Style.  # noqa: E501
 
-        Gets or sets the character formatting of the style.  # noqa: E501
+        Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style.  # noqa: E501
 
-        :return: The font of this Style.  # noqa: E501
-        :rtype: Font
+        :return: The next_paragraph_style_name of this Style.  # noqa: E501
+        :rtype: str
         """
-        return self._font
+        return self._next_paragraph_style_name
 
-    @font.setter
-    def font(self, font):
-        """Sets the font of this Style.
+    @next_paragraph_style_name.setter
+    def next_paragraph_style_name(self, next_paragraph_style_name):
+        """Sets the next_paragraph_style_name of this Style.
 
-        Gets or sets the character formatting of the style.  # noqa: E501
+        Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style.  # noqa: E501
 
-        :param font: The font of this Style.  # noqa: E501
-        :type: Font
+        :param next_paragraph_style_name: The next_paragraph_style_name of this Style.  # noqa: E501
+        :type: str
         """
-        self._font = font
+        self._next_paragraph_style_name = next_paragraph_style_name
 
     @property
-    def is_heading(self):
-        """Gets the is_heading of this Style.  # noqa: E501
+    def base_style_name(self):
+        """Gets the base_style_name of this Style.  # noqa: E501
 
-        Gets or sets a value indicating whether the style is one of the built-in Heading styles.  # noqa: E501
+        Gets or sets the name of the style this style is based on.  # noqa: E501
 
-        :return: The is_heading of this Style.  # noqa: E501
-        :rtype: bool
+        :return: The base_style_name of this Style.  # noqa: E501
+        :rtype: str
         """
-        return self._is_heading
+        return self._base_style_name
 
-    @is_heading.setter
-    def is_heading(self, is_heading):
-        """Sets the is_heading of this Style.
+    @base_style_name.setter
+    def base_style_name(self, base_style_name):
+        """Sets the base_style_name of this Style.
 
-        Gets or sets a value indicating whether the style is one of the built-in Heading styles.  # noqa: E501
+        Gets or sets the name of the style this style is based on.  # noqa: E501
 
-        :param is_heading: The is_heading of this Style.  # noqa: E501
-        :type: bool
+        :param base_style_name: The base_style_name of this Style.  # noqa: E501
+        :type: str
         """
-        self._is_heading = is_heading
+        self._base_style_name = base_style_name
 
     @property
     def is_quick_style(self):
         """Gets the is_quick_style of this Style.  # noqa: E501
 
         Gets or sets a value indicating whether this style is shown in the Quick Style gallery inside MS Word UI.  # noqa: E501
 
@@ -286,56 +264,86 @@
 
         :param linked_style_name: The linked_style_name of this Style.  # noqa: E501
         :type: str
         """
         self._linked_style_name = linked_style_name
 
     @property
-    def name(self):
-        """Gets the name of this Style.  # noqa: E501
+    def type(self):
+        """Gets the type of this Style.  # noqa: E501
 
-        Gets or sets the name of the style.  # noqa: E501
+        Gets or sets the style type (paragraph or character).  # noqa: E501
 
-        :return: The name of this Style.  # noqa: E501
+        :return: The type of this Style.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this Style.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this Style.
 
-        Gets or sets the name of the style.  # noqa: E501
+        Gets or sets the style type (paragraph or character).  # noqa: E501
 
-        :param name: The name of this Style.  # noqa: E501
+        :param type: The type of this Style.  # noqa: E501
         :type: str
         """
-        self._name = name
+        allowed_values = ["Paragraph", "Character", "Table", "List"]  # noqa: E501
+        if not type.isdigit():
+            if type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(type, allowed_values))
+            self._type = type
+        else:
+            self._type = allowed_values[int(type) if six.PY3 else long(type)]
 
     @property
-    def next_paragraph_style_name(self):
-        """Gets the next_paragraph_style_name of this Style.  # noqa: E501
+    def is_heading(self):
+        """Gets the is_heading of this Style.  # noqa: E501
 
-        Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style.  # noqa: E501
+        Gets or sets a value indicating whether the style is one of the built-in Heading styles.  # noqa: E501
 
-        :return: The next_paragraph_style_name of this Style.  # noqa: E501
-        :rtype: str
+        :return: The is_heading of this Style.  # noqa: E501
+        :rtype: bool
         """
-        return self._next_paragraph_style_name
+        return self._is_heading
 
-    @next_paragraph_style_name.setter
-    def next_paragraph_style_name(self, next_paragraph_style_name):
-        """Sets the next_paragraph_style_name of this Style.
+    @is_heading.setter
+    def is_heading(self, is_heading):
+        """Sets the is_heading of this Style.
 
-        Gets or sets the name of the style to be applied automatically to a new paragraph inserted after a paragraph formatted with the specified style.  # noqa: E501
+        Gets or sets a value indicating whether the style is one of the built-in Heading styles.  # noqa: E501
 
-        :param next_paragraph_style_name: The next_paragraph_style_name of this Style.  # noqa: E501
-        :type: str
+        :param is_heading: The is_heading of this Style.  # noqa: E501
+        :type: bool
         """
-        self._next_paragraph_style_name = next_paragraph_style_name
+        self._is_heading = is_heading
+
+    @property
+    def aliases(self):
+        """Gets the aliases of this Style.  # noqa: E501
+
+        Gets or sets all aliases of this style. If style has no aliases then empty array of string is returned.  # noqa: E501
+
+        :return: The aliases of this Style.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._aliases
+
+    @aliases.setter
+    def aliases(self, aliases):
+        """Sets the aliases of this Style.
+
+        Gets or sets all aliases of this style. If style has no aliases then empty array of string is returned.  # noqa: E501
+
+        :param aliases: The aliases of this Style.  # noqa: E501
+        :type: list[str]
+        """
+        self._aliases = aliases
 
     @property
     def style_identifier(self):
         """Gets the style_identifier of this Style.  # noqa: E501
 
         Gets or sets the locale independent style identifier for a built-in style.  # noqa: E501
 
@@ -360,42 +368,34 @@
                     "Invalid value for `style_identifier` ({0}), must be one of {1}"  # noqa: E501
                     .format(style_identifier, allowed_values))
             self._style_identifier = style_identifier
         else:
             self._style_identifier = allowed_values[int(style_identifier) if six.PY3 else long(style_identifier)]
 
     @property
-    def type(self):
-        """Gets the type of this Style.  # noqa: E501
+    def name(self):
+        """Gets the name of this Style.  # noqa: E501
 
-        Gets or sets the style type (paragraph or character).  # noqa: E501
+        Gets or sets the name of the style.  # noqa: E501
 
-        :return: The type of this Style.  # noqa: E501
+        :return: The name of this Style.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._name
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this Style.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this Style.
 
-        Gets or sets the style type (paragraph or character).  # noqa: E501
+        Gets or sets the name of the style.  # noqa: E501
 
-        :param type: The type of this Style.  # noqa: E501
+        :param name: The name of this Style.  # noqa: E501
         :type: str
         """
-        allowed_values = ["Paragraph", "Character", "Table", "List"]  # noqa: E501
-        if not type.isdigit():
-            if type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(type, allowed_values))
-            self._type = type
-        else:
-            self._type = allowed_values[int(type) if six.PY3 else long(type)]
+        self._name = name
 
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/dotx_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/dotx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/tiff_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/tiff_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,21 +67,21 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
-        'save_format': 'str',
+        'use_gdi_emf_renderer': 'bool',
         'threshold_for_floyd_steinberg_dithering': 'int',
         'tiff_binarization_method': 'str',
-        'tiff_compression': 'str'
+        'tiff_compression': 'str',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -106,24 +106,24 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
-        'save_format': 'SaveFormat',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'threshold_for_floyd_steinberg_dithering': 'ThresholdForFloydSteinbergDithering',
         'tiff_binarization_method': 'TiffBinarizationMethod',
-        'tiff_compression': 'TiffCompression'
+        'tiff_compression': 'TiffCompression',
+        'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None, threshold_for_floyd_steinberg_dithering=None, tiff_binarization_method=None, tiff_compression=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None, threshold_for_floyd_steinberg_dithering=None, tiff_binarization_method=None, tiff_compression=None):  # noqa: E501
         """TiffSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -147,21 +147,21 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
-        self._save_format = "tiff"
+        self._use_gdi_emf_renderer = None
         self._threshold_for_floyd_steinberg_dithering = None
         self._tiff_binarization_method = None
         self._tiff_compression = None
+        self._save_format = "tiff"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -214,20 +214,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if threshold_for_floyd_steinberg_dithering is not None:
             self.threshold_for_floyd_steinberg_dithering = threshold_for_floyd_steinberg_dithering
         if tiff_binarization_method is not None:
             self.tiff_binarization_method = tiff_binarization_method
         if tiff_compression is not None:
             self.tiff_compression = tiff_compression
 
@@ -930,36 +930,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this TiffSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this TiffSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this TiffSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this TiffSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -996,24 +974,34 @@
 
         :param vertical_resolution: The vertical_resolution of this TiffSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
-    def save_format(self):
-        """Gets the save_format of this TiffSaveOptionsData.  # noqa: E501
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
 
-        Gets the format of save.  # noqa: E501
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
 
-        :return: The save_format of this TiffSaveOptionsData.  # noqa: E501
-        :rtype: str
+        :return: The use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
+        :rtype: bool
         """
-        return self._save_format
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this TiffSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
 
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this TiffSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def threshold_for_floyd_steinberg_dithering(self):
         """Gets the threshold_for_floyd_steinberg_dithering of this TiffSaveOptionsData.  # noqa: E501
 
         Gets or sets the threshold that determines the value of the binarization error in the Floyd-Steinberg method. when ImageBinarizationMethod is ImageBinarizationMethod.FloydSteinbergDithering. Default value is 128.  # noqa: E501
 
@@ -1089,14 +1077,26 @@
                 raise ValueError(
                     "Invalid value for `tiff_compression` ({0}), must be one of {1}"  # noqa: E501
                     .format(tiff_compression, allowed_values))
             self._tiff_compression = tiff_compression
         else:
             self._tiff_compression = allowed_values[int(tiff_compression) if six.PY3 else long(tiff_compression)]
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this TiffSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this TiffSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/save_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/run_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/run_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/epub_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/epub_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_list_format_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_list_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/new_document_position.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/new_document_position.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xml_data_load_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xml_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/ott_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/ott_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_objects_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_objects_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_insert_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlinks_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks_outline_level_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks_outline_level_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,150 +40,150 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'appearance': 'str',
-        'building_block_category': 'str',
-        'building_block_gallery': 'str',
-        'calendar_type': 'str',
+        'list_items': 'list[StructuredDocumentTagListItem]',
         'checked': 'bool',
-        'color': 'str',
-        'date_display_format': 'str',
+        'appearance': 'str',
         'date_display_locale': 'int',
-        'date_storage_format': 'str',
+        'date_display_format': 'str',
         'full_date': 'datetime',
-        'id': 'int',
-        'is_showing_placeholder_text': 'bool',
+        'title': 'str',
+        'date_storage_format': 'str',
+        'building_block_gallery': 'str',
+        'building_block_category': 'str',
+        'multiline': 'bool',
+        'color': 'str',
+        'style_name': 'str',
+        'calendar_type': 'str',
         'is_temporary': 'bool',
         'level': 'str',
-        'list_items': 'list[StructuredDocumentTagListItem]',
+        'sdt_type': 'str',
+        'placeholder_name': 'str',
         'lock_content_control': 'bool',
         'lock_contents': 'bool',
-        'multiline': 'bool',
-        'placeholder_name': 'str',
-        'sdt_type': 'str',
-        'style_name': 'str',
+        'is_showing_placeholder_text': 'bool',
         'tag': 'str',
-        'title': 'str',
+        'id': 'int',
         'word_open_xml': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'appearance': 'Appearance',
-        'building_block_category': 'BuildingBlockCategory',
-        'building_block_gallery': 'BuildingBlockGallery',
-        'calendar_type': 'CalendarType',
+        'list_items': 'ListItems',
         'checked': 'Checked',
-        'color': 'Color',
-        'date_display_format': 'DateDisplayFormat',
+        'appearance': 'Appearance',
         'date_display_locale': 'DateDisplayLocale',
-        'date_storage_format': 'DateStorageFormat',
+        'date_display_format': 'DateDisplayFormat',
         'full_date': 'FullDate',
-        'id': 'Id',
-        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
+        'title': 'Title',
+        'date_storage_format': 'DateStorageFormat',
+        'building_block_gallery': 'BuildingBlockGallery',
+        'building_block_category': 'BuildingBlockCategory',
+        'multiline': 'Multiline',
+        'color': 'Color',
+        'style_name': 'StyleName',
+        'calendar_type': 'CalendarType',
         'is_temporary': 'IsTemporary',
         'level': 'Level',
-        'list_items': 'ListItems',
+        'sdt_type': 'SdtType',
+        'placeholder_name': 'PlaceholderName',
         'lock_content_control': 'LockContentControl',
         'lock_contents': 'LockContents',
-        'multiline': 'Multiline',
-        'placeholder_name': 'PlaceholderName',
-        'sdt_type': 'SdtType',
-        'style_name': 'StyleName',
+        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
         'tag': 'Tag',
-        'title': 'Title',
+        'id': 'Id',
         'word_open_xml': 'WordOpenXML'
     }
 
-    def __init__(self, link=None, node_id=None, appearance=None, building_block_category=None, building_block_gallery=None, calendar_type=None, checked=None, color=None, date_display_format=None, date_display_locale=None, date_storage_format=None, full_date=None, id=None, is_showing_placeholder_text=None, is_temporary=None, level=None, list_items=None, lock_content_control=None, lock_contents=None, multiline=None, placeholder_name=None, sdt_type=None, style_name=None, tag=None, title=None, word_open_xml=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, list_items=None, checked=None, appearance=None, date_display_locale=None, date_display_format=None, full_date=None, title=None, date_storage_format=None, building_block_gallery=None, building_block_category=None, multiline=None, color=None, style_name=None, calendar_type=None, is_temporary=None, level=None, sdt_type=None, placeholder_name=None, lock_content_control=None, lock_contents=None, is_showing_placeholder_text=None, tag=None, id=None, word_open_xml=None):  # noqa: E501
         """StructuredDocumentTagUpdate - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._appearance = None
-        self._building_block_category = None
-        self._building_block_gallery = None
-        self._calendar_type = None
+        self._list_items = None
         self._checked = None
-        self._color = None
-        self._date_display_format = None
+        self._appearance = None
         self._date_display_locale = None
-        self._date_storage_format = None
+        self._date_display_format = None
         self._full_date = None
-        self._id = None
-        self._is_showing_placeholder_text = None
+        self._title = None
+        self._date_storage_format = None
+        self._building_block_gallery = None
+        self._building_block_category = None
+        self._multiline = None
+        self._color = None
+        self._style_name = None
+        self._calendar_type = None
         self._is_temporary = None
         self._level = None
-        self._list_items = None
+        self._sdt_type = None
+        self._placeholder_name = None
         self._lock_content_control = None
         self._lock_contents = None
-        self._multiline = None
-        self._placeholder_name = None
-        self._sdt_type = None
-        self._style_name = None
+        self._is_showing_placeholder_text = None
         self._tag = None
-        self._title = None
+        self._id = None
         self._word_open_xml = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if appearance is not None:
-            self.appearance = appearance
-        if building_block_category is not None:
-            self.building_block_category = building_block_category
-        if building_block_gallery is not None:
-            self.building_block_gallery = building_block_gallery
-        if calendar_type is not None:
-            self.calendar_type = calendar_type
+        if list_items is not None:
+            self.list_items = list_items
         if checked is not None:
             self.checked = checked
-        if color is not None:
-            self.color = color
-        if date_display_format is not None:
-            self.date_display_format = date_display_format
+        if appearance is not None:
+            self.appearance = appearance
         if date_display_locale is not None:
             self.date_display_locale = date_display_locale
-        if date_storage_format is not None:
-            self.date_storage_format = date_storage_format
+        if date_display_format is not None:
+            self.date_display_format = date_display_format
         if full_date is not None:
             self.full_date = full_date
-        if id is not None:
-            self.id = id
-        if is_showing_placeholder_text is not None:
-            self.is_showing_placeholder_text = is_showing_placeholder_text
+        if title is not None:
+            self.title = title
+        if date_storage_format is not None:
+            self.date_storage_format = date_storage_format
+        if building_block_gallery is not None:
+            self.building_block_gallery = building_block_gallery
+        if building_block_category is not None:
+            self.building_block_category = building_block_category
+        if multiline is not None:
+            self.multiline = multiline
+        if color is not None:
+            self.color = color
+        if style_name is not None:
+            self.style_name = style_name
+        if calendar_type is not None:
+            self.calendar_type = calendar_type
         if is_temporary is not None:
             self.is_temporary = is_temporary
         if level is not None:
             self.level = level
-        if list_items is not None:
-            self.list_items = list_items
+        if sdt_type is not None:
+            self.sdt_type = sdt_type
+        if placeholder_name is not None:
+            self.placeholder_name = placeholder_name
         if lock_content_control is not None:
             self.lock_content_control = lock_content_control
         if lock_contents is not None:
             self.lock_contents = lock_contents
-        if multiline is not None:
-            self.multiline = multiline
-        if placeholder_name is not None:
-            self.placeholder_name = placeholder_name
-        if sdt_type is not None:
-            self.sdt_type = sdt_type
-        if style_name is not None:
-            self.style_name = style_name
+        if is_showing_placeholder_text is not None:
+            self.is_showing_placeholder_text = is_showing_placeholder_text
         if tag is not None:
             self.tag = tag
-        if title is not None:
-            self.title = title
+        if id is not None:
+            self.id = id
         if word_open_xml is not None:
             self.word_open_xml = word_open_xml
 
     @property
     def link(self):
         """Gets the link of this StructuredDocumentTagUpdate.  # noqa: E501
 
@@ -224,14 +224,58 @@
 
         :param node_id: The node_id of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
+    def list_items(self):
+        """Gets the list_items of this StructuredDocumentTagUpdate.  # noqa: E501
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :return: The list_items of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: list[StructuredDocumentTagListItem]
+        """
+        return self._list_items
+
+    @list_items.setter
+    def list_items(self, list_items):
+        """Sets the list_items of this StructuredDocumentTagUpdate.
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :param list_items: The list_items of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: list[StructuredDocumentTagListItem]
+        """
+        self._list_items = list_items
+
+    @property
+    def checked(self):
+        """Gets the checked of this StructuredDocumentTagUpdate.  # noqa: E501
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :return: The checked of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: bool
+        """
+        return self._checked
+
+    @checked.setter
+    def checked(self, checked):
+        """Sets the checked of this StructuredDocumentTagUpdate.
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :param checked: The checked of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: bool
+        """
+        self._checked = checked
+
+    @property
     def appearance(self):
         """Gets the appearance of this StructuredDocumentTagUpdate.  # noqa: E501
 
         Gets or sets the appearance of a structured document tag.  # noqa: E501
 
         :return: The appearance of this StructuredDocumentTagUpdate.  # noqa: E501
         :rtype: str
@@ -254,270 +298,270 @@
                     "Invalid value for `appearance` ({0}), must be one of {1}"  # noqa: E501
                     .format(appearance, allowed_values))
             self._appearance = appearance
         else:
             self._appearance = allowed_values[int(appearance) if six.PY3 else long(appearance)]
 
     @property
-    def building_block_category(self):
-        """Gets the building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
+    def date_display_locale(self):
+        """Gets the date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :return: The building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
+        :return: The date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: int
         """
-        return self._building_block_category
+        return self._date_display_locale
 
-    @building_block_category.setter
-    def building_block_category(self, building_block_category):
-        """Sets the building_block_category of this StructuredDocumentTagUpdate.
+    @date_display_locale.setter
+    def date_display_locale(self, date_display_locale):
+        """Sets the date_display_locale of this StructuredDocumentTagUpdate.
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :param building_block_category: The building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
+        :param date_display_locale: The date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: int
         """
-        self._building_block_category = building_block_category
+        self._date_display_locale = date_display_locale
 
     @property
-    def building_block_gallery(self):
-        """Gets the building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
+    def date_display_format(self):
+        """Gets the date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :return: The building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
+        :return: The date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
         :rtype: str
         """
-        return self._building_block_gallery
+        return self._date_display_format
 
-    @building_block_gallery.setter
-    def building_block_gallery(self, building_block_gallery):
-        """Sets the building_block_gallery of this StructuredDocumentTagUpdate.
+    @date_display_format.setter
+    def date_display_format(self, date_display_format):
+        """Sets the date_display_format of this StructuredDocumentTagUpdate.
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
+        :param date_display_format: The date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: str
         """
-        self._building_block_gallery = building_block_gallery
+        self._date_display_format = date_display_format
 
     @property
-    def calendar_type(self):
-        """Gets the calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
+    def full_date(self):
+        """Gets the full_date of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :return: The calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
+        :return: The full_date of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: datetime
         """
-        return self._calendar_type
+        return self._full_date
 
-    @calendar_type.setter
-    def calendar_type(self, calendar_type):
-        """Sets the calendar_type of this StructuredDocumentTagUpdate.
+    @full_date.setter
+    def full_date(self, full_date):
+        """Sets the full_date of this StructuredDocumentTagUpdate.
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :param calendar_type: The calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
+        :param full_date: The full_date of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: datetime
         """
-        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
-        if not calendar_type.isdigit():
-            if calendar_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(calendar_type, allowed_values))
-            self._calendar_type = calendar_type
-        else:
-            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
+        self._full_date = full_date
 
     @property
-    def checked(self):
-        """Gets the checked of this StructuredDocumentTagUpdate.  # noqa: E501
+    def title(self):
+        """Gets the title of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :return: The checked of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: bool
+        :return: The title of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._checked
+        return self._title
 
-    @checked.setter
-    def checked(self, checked):
-        """Sets the checked of this StructuredDocumentTagUpdate.
+    @title.setter
+    def title(self, title):
+        """Sets the title of this StructuredDocumentTagUpdate.
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :param checked: The checked of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: bool
+        :param title: The title of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._checked = checked
+        self._title = title
 
     @property
-    def color(self):
-        """Gets the color of this StructuredDocumentTagUpdate.  # noqa: E501
+    def date_storage_format(self):
+        """Gets the date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :return: The color of this StructuredDocumentTagUpdate.  # noqa: E501
+        :return: The date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
         :rtype: str
         """
-        return self._color
+        return self._date_storage_format
 
-    @color.setter
-    def color(self, color):
-        """Sets the color of this StructuredDocumentTagUpdate.
+    @date_storage_format.setter
+    def date_storage_format(self, date_storage_format):
+        """Sets the date_storage_format of this StructuredDocumentTagUpdate.
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :param color: The color of this StructuredDocumentTagUpdate.  # noqa: E501
+        :param date_storage_format: The date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: str
         """
-        self._color = color
+        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
+        if not date_storage_format.isdigit():
+            if date_storage_format not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
+                    .format(date_storage_format, allowed_values))
+            self._date_storage_format = date_storage_format
+        else:
+            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
 
     @property
-    def date_display_format(self):
-        """Gets the date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
+    def building_block_gallery(self):
+        """Gets the building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :return: The date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
+        :return: The building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
         :rtype: str
         """
-        return self._date_display_format
+        return self._building_block_gallery
 
-    @date_display_format.setter
-    def date_display_format(self, date_display_format):
-        """Sets the date_display_format of this StructuredDocumentTagUpdate.
+    @building_block_gallery.setter
+    def building_block_gallery(self, building_block_gallery):
+        """Sets the building_block_gallery of this StructuredDocumentTagUpdate.
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :param date_display_format: The date_display_format of this StructuredDocumentTagUpdate.  # noqa: E501
+        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: str
         """
-        self._date_display_format = date_display_format
+        self._building_block_gallery = building_block_gallery
 
     @property
-    def date_display_locale(self):
-        """Gets the date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
+    def building_block_category(self):
+        """Gets the building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :return: The date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: int
+        :return: The building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._date_display_locale
+        return self._building_block_category
 
-    @date_display_locale.setter
-    def date_display_locale(self, date_display_locale):
-        """Sets the date_display_locale of this StructuredDocumentTagUpdate.
+    @building_block_category.setter
+    def building_block_category(self, building_block_category):
+        """Sets the building_block_category of this StructuredDocumentTagUpdate.
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :param date_display_locale: The date_display_locale of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: int
+        :param building_block_category: The building_block_category of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._date_display_locale = date_display_locale
+        self._building_block_category = building_block_category
 
     @property
-    def date_storage_format(self):
-        """Gets the date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
+    def multiline(self):
+        """Gets the multiline of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :return: The date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
+        :return: The multiline of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: bool
         """
-        return self._date_storage_format
+        return self._multiline
 
-    @date_storage_format.setter
-    def date_storage_format(self, date_storage_format):
-        """Sets the date_storage_format of this StructuredDocumentTagUpdate.
+    @multiline.setter
+    def multiline(self, multiline):
+        """Sets the multiline of this StructuredDocumentTagUpdate.
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :param date_storage_format: The date_storage_format of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
+        :param multiline: The multiline of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: bool
         """
-        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
-        if not date_storage_format.isdigit():
-            if date_storage_format not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
-                    .format(date_storage_format, allowed_values))
-            self._date_storage_format = date_storage_format
-        else:
-            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
+        self._multiline = multiline
 
     @property
-    def full_date(self):
-        """Gets the full_date of this StructuredDocumentTagUpdate.  # noqa: E501
+    def color(self):
+        """Gets the color of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :return: The full_date of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: datetime
+        :return: The color of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._full_date
+        return self._color
 
-    @full_date.setter
-    def full_date(self, full_date):
-        """Sets the full_date of this StructuredDocumentTagUpdate.
+    @color.setter
+    def color(self, color):
+        """Sets the color of this StructuredDocumentTagUpdate.
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :param full_date: The full_date of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: datetime
+        :param color: The color of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._full_date = full_date
+        self._color = color
 
     @property
-    def id(self):
-        """Gets the id of this StructuredDocumentTagUpdate.  # noqa: E501
+    def style_name(self):
+        """Gets the style_name of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :return: The id of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: int
+        :return: The style_name of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._id
+        return self._style_name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this StructuredDocumentTagUpdate.
+    @style_name.setter
+    def style_name(self, style_name):
+        """Sets the style_name of this StructuredDocumentTagUpdate.
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :param id: The id of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: int
+        :param style_name: The style_name of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._id = id
+        self._style_name = style_name
 
     @property
-    def is_showing_placeholder_text(self):
-        """Gets the is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
+    def calendar_type(self):
+        """Gets the calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :return: The is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: bool
+        :return: The calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._is_showing_placeholder_text
+        return self._calendar_type
 
-    @is_showing_placeholder_text.setter
-    def is_showing_placeholder_text(self, is_showing_placeholder_text):
-        """Sets the is_showing_placeholder_text of this StructuredDocumentTagUpdate.
+    @calendar_type.setter
+    def calendar_type(self, calendar_type):
+        """Sets the calendar_type of this StructuredDocumentTagUpdate.
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: bool
+        :param calendar_type: The calendar_type of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._is_showing_placeholder_text = is_showing_placeholder_text
+        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
+        if not calendar_type.isdigit():
+            if calendar_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(calendar_type, allowed_values))
+            self._calendar_type = calendar_type
+        else:
+            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
 
     @property
     def is_temporary(self):
         """Gets the is_temporary of this StructuredDocumentTagUpdate.  # noqa: E501
 
         Gets or sets a value indicating whether this SDT shall be removed from the WordProcessingML document when its contents are modified.  # noqa: E501
 
@@ -564,34 +608,64 @@
                     "Invalid value for `level` ({0}), must be one of {1}"  # noqa: E501
                     .format(level, allowed_values))
             self._level = level
         else:
             self._level = allowed_values[int(level) if six.PY3 else long(level)]
 
     @property
-    def list_items(self):
-        """Gets the list_items of this StructuredDocumentTagUpdate.  # noqa: E501
+    def sdt_type(self):
+        """Gets the sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :return: The list_items of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: list[StructuredDocumentTagListItem]
+        :return: The sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
         """
-        return self._list_items
+        return self._sdt_type
 
-    @list_items.setter
-    def list_items(self, list_items):
-        """Sets the list_items of this StructuredDocumentTagUpdate.
+    @sdt_type.setter
+    def sdt_type(self, sdt_type):
+        """Sets the sdt_type of this StructuredDocumentTagUpdate.
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :param list_items: The list_items of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: list[StructuredDocumentTagListItem]
+        :param sdt_type: The sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
         """
-        self._list_items = list_items
+        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
+        if not sdt_type.isdigit():
+            if sdt_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(sdt_type, allowed_values))
+            self._sdt_type = sdt_type
+        else:
+            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
+
+    @property
+    def placeholder_name(self):
+        """Gets the placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :return: The placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: str
+        """
+        return self._placeholder_name
+
+    @placeholder_name.setter
+    def placeholder_name(self, placeholder_name):
+        """Sets the placeholder_name of this StructuredDocumentTagUpdate.
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :param placeholder_name: The placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: str
+        """
+        self._placeholder_name = placeholder_name
 
     @property
     def lock_content_control(self):
         """Gets the lock_content_control of this StructuredDocumentTagUpdate.  # noqa: E501
 
         Gets or sets a value indicating whether, this property will prohibit a user from deleting this SDT.  # noqa: E501
 
@@ -630,108 +704,34 @@
 
         :param lock_contents: The lock_contents of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: bool
         """
         self._lock_contents = lock_contents
 
     @property
-    def multiline(self):
-        """Gets the multiline of this StructuredDocumentTagUpdate.  # noqa: E501
+    def is_showing_placeholder_text(self):
+        """Gets the is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :return: The multiline of this StructuredDocumentTagUpdate.  # noqa: E501
+        :return: The is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
         :rtype: bool
         """
-        return self._multiline
+        return self._is_showing_placeholder_text
 
-    @multiline.setter
-    def multiline(self, multiline):
-        """Sets the multiline of this StructuredDocumentTagUpdate.
+    @is_showing_placeholder_text.setter
+    def is_showing_placeholder_text(self, is_showing_placeholder_text):
+        """Sets the is_showing_placeholder_text of this StructuredDocumentTagUpdate.
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :param multiline: The multiline of this StructuredDocumentTagUpdate.  # noqa: E501
+        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: bool
         """
-        self._multiline = multiline
-
-    @property
-    def placeholder_name(self):
-        """Gets the placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :return: The placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
-        """
-        return self._placeholder_name
-
-    @placeholder_name.setter
-    def placeholder_name(self, placeholder_name):
-        """Sets the placeholder_name of this StructuredDocumentTagUpdate.
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :param placeholder_name: The placeholder_name of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
-        """
-        self._placeholder_name = placeholder_name
-
-    @property
-    def sdt_type(self):
-        """Gets the sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :return: The sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
-        """
-        return self._sdt_type
-
-    @sdt_type.setter
-    def sdt_type(self, sdt_type):
-        """Sets the sdt_type of this StructuredDocumentTagUpdate.
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :param sdt_type: The sdt_type of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
-        if not sdt_type.isdigit():
-            if sdt_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(sdt_type, allowed_values))
-            self._sdt_type = sdt_type
-        else:
-            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
-
-    @property
-    def style_name(self):
-        """Gets the style_name of this StructuredDocumentTagUpdate.  # noqa: E501
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :return: The style_name of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
-        """
-        return self._style_name
-
-    @style_name.setter
-    def style_name(self, style_name):
-        """Sets the style_name of this StructuredDocumentTagUpdate.
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :param style_name: The style_name of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
-        """
-        self._style_name = style_name
+        self._is_showing_placeholder_text = is_showing_placeholder_text
 
     @property
     def tag(self):
         """Gets the tag of this StructuredDocumentTagUpdate.  # noqa: E501
 
         Gets or sets a tag associated with the current SDT node. Can not be null.  # noqa: E501
 
@@ -748,34 +748,34 @@
 
         :param tag: The tag of this StructuredDocumentTagUpdate.  # noqa: E501
         :type: str
         """
         self._tag = tag
 
     @property
-    def title(self):
-        """Gets the title of this StructuredDocumentTagUpdate.  # noqa: E501
+    def id(self):
+        """Gets the id of this StructuredDocumentTagUpdate.  # noqa: E501
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :return: The title of this StructuredDocumentTagUpdate.  # noqa: E501
-        :rtype: str
+        :return: The id of this StructuredDocumentTagUpdate.  # noqa: E501
+        :rtype: int
         """
-        return self._title
+        return self._id
 
-    @title.setter
-    def title(self, title):
-        """Sets the title of this StructuredDocumentTagUpdate.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StructuredDocumentTagUpdate.
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :param title: The title of this StructuredDocumentTagUpdate.  # noqa: E501
-        :type: str
+        :param id: The id of this StructuredDocumentTagUpdate.  # noqa: E501
+        :type: int
         """
-        self._title = title
+        self._id = id
 
     @property
     def word_open_xml(self):
         """Gets the word_open_xml of this StructuredDocumentTagUpdate.  # noqa: E501
 
         Gets a string that represents the XML contained within the node in the Aspose.Words.SaveFormat.FlatOpc format.  # noqa: E501
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnotes_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/split_document_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,61 +38,39 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'pages': 'list[FileLink]',
         'source_document': 'FileLink',
-        'zipped_pages': 'FileLink'
+        'zipped_pages': 'FileLink',
+        'pages': 'list[FileLink]'
     }
 
     attribute_map = {
-        'pages': 'Pages',
         'source_document': 'SourceDocument',
-        'zipped_pages': 'ZippedPages'
+        'zipped_pages': 'ZippedPages',
+        'pages': 'Pages'
     }
 
-    def __init__(self, pages=None, source_document=None, zipped_pages=None):  # noqa: E501
+    def __init__(self, source_document=None, zipped_pages=None, pages=None):  # noqa: E501
         """SplitDocumentResult - a model defined in Swagger"""  # noqa: E501
 
-        self._pages = None
         self._source_document = None
         self._zipped_pages = None
+        self._pages = None
         self.discriminator = None
 
-        if pages is not None:
-            self.pages = pages
         if source_document is not None:
             self.source_document = source_document
         if zipped_pages is not None:
             self.zipped_pages = zipped_pages
-
-    @property
-    def pages(self):
-        """Gets the pages of this SplitDocumentResult.  # noqa: E501
-
-        Gets or sets the list of pages.  # noqa: E501
-
-        :return: The pages of this SplitDocumentResult.  # noqa: E501
-        :rtype: list[FileLink]
-        """
-        return self._pages
-
-    @pages.setter
-    def pages(self, pages):
-        """Sets the pages of this SplitDocumentResult.
-
-        Gets or sets the list of pages.  # noqa: E501
-
-        :param pages: The pages of this SplitDocumentResult.  # noqa: E501
-        :type: list[FileLink]
-        """
-        self._pages = pages
+        if pages is not None:
+            self.pages = pages
 
     @property
     def source_document(self):
         """Gets the source_document of this SplitDocumentResult.  # noqa: E501
 
         Gets or sets the link to the source document.  # noqa: E501
 
@@ -130,14 +108,36 @@
         Gets or sets the link to the file archive with pages.  # noqa: E501
 
         :param zipped_pages: The zipped_pages of this SplitDocumentResult.  # noqa: E501
         :type: FileLink
         """
         self._zipped_pages = zipped_pages
 
+    @property
+    def pages(self):
+        """Gets the pages of this SplitDocumentResult.  # noqa: E501
+
+        Gets or sets the list of pages.  # noqa: E501
+
+        :return: The pages of this SplitDocumentResult.  # noqa: E501
+        :rtype: list[FileLink]
+        """
+        return self._pages
+
+    @pages.setter
+    def pages(self, pages):
+        """Sets the pages of this SplitDocumentResult.
+
+        Gets or sets the list of pages.  # noqa: E501
+
+        :param pages: The pages of this SplitDocumentResult.  # noqa: E501
+        :type: list[FileLink]
+        """
+        self._pages = pages
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tags_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tags_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section_page_setup_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section_page_setup_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlink_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,46 +41,46 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'type': 'str',
         'child_nodes': 'list[NodeLink]',
-        'drawing_objects': 'LinkElement',
-        'paragraphs': 'LinkElement'
+        'paragraphs': 'LinkElement',
+        'drawing_objects': 'LinkElement'
     }
 
     attribute_map = {
         'link': 'Link',
         'type': 'Type',
         'child_nodes': 'ChildNodes',
-        'drawing_objects': 'DrawingObjects',
-        'paragraphs': 'Paragraphs'
+        'paragraphs': 'Paragraphs',
+        'drawing_objects': 'DrawingObjects'
     }
 
-    def __init__(self, link=None, type=None, child_nodes=None, drawing_objects=None, paragraphs=None):  # noqa: E501
+    def __init__(self, link=None, type=None, child_nodes=None, paragraphs=None, drawing_objects=None):  # noqa: E501
         """HeaderFooter - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._type = None
         self._child_nodes = None
-        self._drawing_objects = None
         self._paragraphs = None
+        self._drawing_objects = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if type is not None:
             self.type = type
         if child_nodes is not None:
             self.child_nodes = child_nodes
-        if drawing_objects is not None:
-            self.drawing_objects = drawing_objects
         if paragraphs is not None:
             self.paragraphs = paragraphs
+        if drawing_objects is not None:
+            self.drawing_objects = drawing_objects
 
     @property
     def link(self):
         """Gets the link of this HeaderFooter.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -149,36 +149,14 @@
 
         :param child_nodes: The child_nodes of this HeaderFooter.  # noqa: E501
         :type: list[NodeLink]
         """
         self._child_nodes = child_nodes
 
     @property
-    def drawing_objects(self):
-        """Gets the drawing_objects of this HeaderFooter.  # noqa: E501
-
-        Gets or sets the link to DrawingObjects resource.  # noqa: E501
-
-        :return: The drawing_objects of this HeaderFooter.  # noqa: E501
-        :rtype: LinkElement
-        """
-        return self._drawing_objects
-
-    @drawing_objects.setter
-    def drawing_objects(self, drawing_objects):
-        """Sets the drawing_objects of this HeaderFooter.
-
-        Gets or sets the link to DrawingObjects resource.  # noqa: E501
-
-        :param drawing_objects: The drawing_objects of this HeaderFooter.  # noqa: E501
-        :type: LinkElement
-        """
-        self._drawing_objects = drawing_objects
-
-    @property
     def paragraphs(self):
         """Gets the paragraphs of this HeaderFooter.  # noqa: E501
 
         Gets or sets the link to Paragraphs resource.  # noqa: E501
 
         :return: The paragraphs of this HeaderFooter.  # noqa: E501
         :rtype: LinkElement
@@ -192,14 +170,36 @@
         Gets or sets the link to Paragraphs resource.  # noqa: E501
 
         :param paragraphs: The paragraphs of this HeaderFooter.  # noqa: E501
         :type: LinkElement
         """
         self._paragraphs = paragraphs
 
+    @property
+    def drawing_objects(self):
+        """Gets the drawing_objects of this HeaderFooter.  # noqa: E501
+
+        Gets or sets the link to DrawingObjects resource.  # noqa: E501
+
+        :return: The drawing_objects of this HeaderFooter.  # noqa: E501
+        :rtype: LinkElement
+        """
+        return self._drawing_objects
+
+    @drawing_objects.setter
+    def drawing_objects(self, drawing_objects):
+        """Sets the drawing_objects of this HeaderFooter.
+
+        Gets or sets the link to DrawingObjects resource.  # noqa: E501
+
+        :param drawing_objects: The drawing_objects of this HeaderFooter.  # noqa: E501
+        :type: LinkElement
+        """
+        self._drawing_objects = drawing_objects
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stops_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stops_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/page_setup.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comment_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/markdown_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/markdown_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         'update_last_saved_time_property': 'bool',
         'update_sdt_content': 'bool',
         'zip_output': 'bool',
         'encoding': 'str',
         'export_headers_footers_mode': 'str',
         'force_page_breaks': 'bool',
         'paragraph_break': 'str',
-        'save_format': 'str',
-        'table_content_alignment': 'str'
+        'table_content_alignment': 'str',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -77,16 +77,16 @@
         'update_last_saved_time_property': 'UpdateLastSavedTimeProperty',
         'update_sdt_content': 'UpdateSdtContent',
         'zip_output': 'ZipOutput',
         'encoding': 'Encoding',
         'export_headers_footers_mode': 'ExportHeadersFootersMode',
         'force_page_breaks': 'ForcePageBreaks',
         'paragraph_break': 'ParagraphBreak',
-        'save_format': 'SaveFormat',
-        'table_content_alignment': 'TableContentAlignment'
+        'table_content_alignment': 'TableContentAlignment',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, encoding=None, export_headers_footers_mode=None, force_page_breaks=None, paragraph_break=None, table_content_alignment=None):  # noqa: E501
         """MarkdownSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -101,16 +101,16 @@
         self._update_last_saved_time_property = None
         self._update_sdt_content = None
         self._zip_output = None
         self._encoding = None
         self._export_headers_footers_mode = None
         self._force_page_breaks = None
         self._paragraph_break = None
-        self._save_format = "md"
         self._table_content_alignment = None
+        self._save_format = "md"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -557,26 +557,14 @@
 
         :param paragraph_break: The paragraph_break of this MarkdownSaveOptionsData.  # noqa: E501
         :type: str
         """
         self._paragraph_break = paragraph_break
 
     @property
-    def save_format(self):
-        """Gets the save_format of this MarkdownSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this MarkdownSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def table_content_alignment(self):
         """Gets the table_content_alignment of this MarkdownSaveOptionsData.  # noqa: E501
 
         Gets or sets the value, that specifies how to align contents in tables when exporting into the Markdown format. The default value is Auto.  # noqa: E501
 
         :return: The table_content_alignment of this MarkdownSaveOptionsData.  # noqa: E501
         :rtype: str
@@ -598,14 +586,26 @@
                 raise ValueError(
                     "Invalid value for `table_content_alignment` ({0}), must be one of {1}"  # noqa: E501
                     .format(table_content_alignment, allowed_values))
             self._table_content_alignment = table_content_alignment
         else:
             self._table_content_alignment = allowed_values[int(table_content_alignment) if six.PY3 else long(table_content_alignment)]
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this MarkdownSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this MarkdownSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_header_footer_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_header_footer_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_border_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_page_numbers_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_page_numbers_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_footnote_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_bookmark_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/compress_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compress_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_list_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/compare_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/compare_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_field_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_run_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_section_page_setup_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_section_page_setup_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/protect_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/protect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_style_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_or_update_paragraph_tab_stop_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_run_font_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_font_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_all_paragraph_tab_stops_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_fields_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_fields_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/replace_with_text_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_with_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/replace_text_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/replace_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_row_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_row_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_custom_xml_part_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/reject_all_revisions_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/reject_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_row_format_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_row_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_comment_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_structured_document_tag_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_drawing_object_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_field_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_form_field_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_paragraph_format_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_borders_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_borders_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/remove_range_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/remove_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_bookmark_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_bookmark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/accept_all_revisions_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/accept_all_revisions_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_footnote_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_footnote_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_custom_xml_part_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_paragraph_list_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/__init__.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_comment_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_comment_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_run_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_run_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_cell_format_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_cell_format_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_tiff_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_tiff_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_list_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_style_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/unprotect_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/unprotect_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_form_field_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_form_field_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_border_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_border_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/save_as_range_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/save_as_range_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_table_properties_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_table_properties_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/split_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/split_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_paragraph_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_paragraph_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/copy_style_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/copy_style_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_structured_document_tag_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_list_level_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_list_level_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/delete_watermark_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/delete_watermark_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/apply_style_to_document_element_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_table_cell_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_table_cell_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/update_drawing_object_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/update_drawing_object_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/create_or_update_document_property_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/create_or_update_document_property_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_watermark_text_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_text_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/append_document_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/append_document_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/responses/insert_watermark_image_online_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/responses/insert_watermark_image_online_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/docm_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/docm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/ps_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/ps_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         'color_mode': 'str',
         'jpeg_quality': 'int',
         'metafile_rendering_options': 'MetafileRenderingOptionsData',
         'numeral_format': 'str',
         'optimize_output': 'bool',
         'page_count': 'int',
         'page_index': 'int',
-        'save_format': 'str',
-        'use_book_fold_printing_settings': 'bool'
+        'use_book_fold_printing_settings': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -83,16 +83,16 @@
         'color_mode': 'ColorMode',
         'jpeg_quality': 'JpegQuality',
         'metafile_rendering_options': 'MetafileRenderingOptions',
         'numeral_format': 'NumeralFormat',
         'optimize_output': 'OptimizeOutput',
         'page_count': 'PageCount',
         'page_index': 'PageIndex',
-        'save_format': 'SaveFormat',
-        'use_book_fold_printing_settings': 'UseBookFoldPrintingSettings'
+        'use_book_fold_printing_settings': 'UseBookFoldPrintingSettings',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, use_book_fold_printing_settings=None):  # noqa: E501
         """PsSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -110,16 +110,16 @@
         self._color_mode = None
         self._jpeg_quality = None
         self._metafile_rendering_options = None
         self._numeral_format = None
         self._optimize_output = None
         self._page_count = None
         self._page_index = None
-        self._save_format = "ps"
         self._use_book_fold_printing_settings = None
+        self._save_format = "ps"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -646,26 +646,14 @@
 
         :param page_index: The page_index of this PsSaveOptionsData.  # noqa: E501
         :type: int
         """
         self._page_index = page_index
 
     @property
-    def save_format(self):
-        """Gets the save_format of this PsSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this PsSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def use_book_fold_printing_settings(self):
         """Gets the use_book_fold_printing_settings of this PsSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether the document should be saved using a booklet printing layout.  # noqa: E501
 
         :return: The use_book_fold_printing_settings of this PsSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -679,14 +667,26 @@
         Gets or sets a value indicating whether the document should be saved using a booklet printing layout.  # noqa: E501
 
         :param use_book_fold_printing_settings: The use_book_fold_printing_settings of this PsSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_book_fold_printing_settings = use_book_fold_printing_settings
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this PsSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this PsSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comments_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comments_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/dotm_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/dotm_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_link_collection_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlinks.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xml_color.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xml_color.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,38 +39,38 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'data': 'str',
-        'id': 'str'
+        'id': 'str',
+        'data': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
-        'data': 'Data',
-        'id': 'Id'
+        'id': 'Id',
+        'data': 'Data'
     }
 
-    def __init__(self, link=None, data=None, id=None):  # noqa: E501
+    def __init__(self, link=None, id=None, data=None):  # noqa: E501
         """CustomXmlPartUpdate - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._data = None
         self._id = None
+        self._data = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if data is not None:
-            self.data = data
         if id is not None:
             self.id = id
+        if data is not None:
+            self.data = data
 
     @property
     def link(self):
         """Gets the link of this CustomXmlPartUpdate.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -87,36 +87,14 @@
 
         :param link: The link of this CustomXmlPartUpdate.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def data(self):
-        """Gets the data of this CustomXmlPartUpdate.  # noqa: E501
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :return: The data of this CustomXmlPartUpdate.  # noqa: E501
-        :rtype: str
-        """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this CustomXmlPartUpdate.
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :param data: The data of this CustomXmlPartUpdate.  # noqa: E501
-        :type: str
-        """
-        self._data = data
-
-    @property
     def id(self):
         """Gets the id of this CustomXmlPartUpdate.  # noqa: E501
 
         Gets or sets the custom xml part id.  # noqa: E501
 
         :return: The id of this CustomXmlPartUpdate.  # noqa: E501
         :rtype: str
@@ -130,14 +108,36 @@
         Gets or sets the custom xml part id.  # noqa: E501
 
         :param id: The id of this CustomXmlPartUpdate.  # noqa: E501
         :type: str
         """
         self._id = id
 
+    @property
+    def data(self):
+        """Gets the data of this CustomXmlPartUpdate.  # noqa: E501
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :return: The data of this CustomXmlPartUpdate.  # noqa: E501
+        :rtype: str
+        """
+        return self._data
+
+    @data.setter
+    def data(self, data):
+        """Sets the data of this CustomXmlPartUpdate.
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :param data: The data of this CustomXmlPartUpdate.  # noqa: E501
+        :type: str
+        """
+        self._data = data
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,150 +40,150 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'appearance': 'str',
-        'building_block_category': 'str',
-        'building_block_gallery': 'str',
-        'calendar_type': 'str',
+        'list_items': 'list[StructuredDocumentTagListItem]',
         'checked': 'bool',
-        'color': 'str',
-        'date_display_format': 'str',
+        'appearance': 'str',
         'date_display_locale': 'int',
-        'date_storage_format': 'str',
+        'date_display_format': 'str',
         'full_date': 'datetime',
-        'id': 'int',
-        'is_showing_placeholder_text': 'bool',
+        'title': 'str',
+        'date_storage_format': 'str',
+        'building_block_gallery': 'str',
+        'building_block_category': 'str',
+        'multiline': 'bool',
+        'color': 'str',
+        'style_name': 'str',
+        'calendar_type': 'str',
         'is_temporary': 'bool',
         'level': 'str',
-        'list_items': 'list[StructuredDocumentTagListItem]',
+        'sdt_type': 'str',
+        'placeholder_name': 'str',
         'lock_content_control': 'bool',
         'lock_contents': 'bool',
-        'multiline': 'bool',
-        'placeholder_name': 'str',
-        'sdt_type': 'str',
-        'style_name': 'str',
+        'is_showing_placeholder_text': 'bool',
         'tag': 'str',
-        'title': 'str',
+        'id': 'int',
         'word_open_xml': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'appearance': 'Appearance',
-        'building_block_category': 'BuildingBlockCategory',
-        'building_block_gallery': 'BuildingBlockGallery',
-        'calendar_type': 'CalendarType',
+        'list_items': 'ListItems',
         'checked': 'Checked',
-        'color': 'Color',
-        'date_display_format': 'DateDisplayFormat',
+        'appearance': 'Appearance',
         'date_display_locale': 'DateDisplayLocale',
-        'date_storage_format': 'DateStorageFormat',
+        'date_display_format': 'DateDisplayFormat',
         'full_date': 'FullDate',
-        'id': 'Id',
-        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
+        'title': 'Title',
+        'date_storage_format': 'DateStorageFormat',
+        'building_block_gallery': 'BuildingBlockGallery',
+        'building_block_category': 'BuildingBlockCategory',
+        'multiline': 'Multiline',
+        'color': 'Color',
+        'style_name': 'StyleName',
+        'calendar_type': 'CalendarType',
         'is_temporary': 'IsTemporary',
         'level': 'Level',
-        'list_items': 'ListItems',
+        'sdt_type': 'SdtType',
+        'placeholder_name': 'PlaceholderName',
         'lock_content_control': 'LockContentControl',
         'lock_contents': 'LockContents',
-        'multiline': 'Multiline',
-        'placeholder_name': 'PlaceholderName',
-        'sdt_type': 'SdtType',
-        'style_name': 'StyleName',
+        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
         'tag': 'Tag',
-        'title': 'Title',
+        'id': 'Id',
         'word_open_xml': 'WordOpenXML'
     }
 
-    def __init__(self, link=None, node_id=None, appearance=None, building_block_category=None, building_block_gallery=None, calendar_type=None, checked=None, color=None, date_display_format=None, date_display_locale=None, date_storage_format=None, full_date=None, id=None, is_showing_placeholder_text=None, is_temporary=None, level=None, list_items=None, lock_content_control=None, lock_contents=None, multiline=None, placeholder_name=None, sdt_type=None, style_name=None, tag=None, title=None, word_open_xml=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, list_items=None, checked=None, appearance=None, date_display_locale=None, date_display_format=None, full_date=None, title=None, date_storage_format=None, building_block_gallery=None, building_block_category=None, multiline=None, color=None, style_name=None, calendar_type=None, is_temporary=None, level=None, sdt_type=None, placeholder_name=None, lock_content_control=None, lock_contents=None, is_showing_placeholder_text=None, tag=None, id=None, word_open_xml=None):  # noqa: E501
         """StructuredDocumentTag - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._appearance = None
-        self._building_block_category = None
-        self._building_block_gallery = None
-        self._calendar_type = None
+        self._list_items = None
         self._checked = None
-        self._color = None
-        self._date_display_format = None
+        self._appearance = None
         self._date_display_locale = None
-        self._date_storage_format = None
+        self._date_display_format = None
         self._full_date = None
-        self._id = None
-        self._is_showing_placeholder_text = None
+        self._title = None
+        self._date_storage_format = None
+        self._building_block_gallery = None
+        self._building_block_category = None
+        self._multiline = None
+        self._color = None
+        self._style_name = None
+        self._calendar_type = None
         self._is_temporary = None
         self._level = None
-        self._list_items = None
+        self._sdt_type = None
+        self._placeholder_name = None
         self._lock_content_control = None
         self._lock_contents = None
-        self._multiline = None
-        self._placeholder_name = None
-        self._sdt_type = None
-        self._style_name = None
+        self._is_showing_placeholder_text = None
         self._tag = None
-        self._title = None
+        self._id = None
         self._word_open_xml = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if appearance is not None:
-            self.appearance = appearance
-        if building_block_category is not None:
-            self.building_block_category = building_block_category
-        if building_block_gallery is not None:
-            self.building_block_gallery = building_block_gallery
-        if calendar_type is not None:
-            self.calendar_type = calendar_type
+        if list_items is not None:
+            self.list_items = list_items
         if checked is not None:
             self.checked = checked
-        if color is not None:
-            self.color = color
-        if date_display_format is not None:
-            self.date_display_format = date_display_format
+        if appearance is not None:
+            self.appearance = appearance
         if date_display_locale is not None:
             self.date_display_locale = date_display_locale
-        if date_storage_format is not None:
-            self.date_storage_format = date_storage_format
+        if date_display_format is not None:
+            self.date_display_format = date_display_format
         if full_date is not None:
             self.full_date = full_date
-        if id is not None:
-            self.id = id
-        if is_showing_placeholder_text is not None:
-            self.is_showing_placeholder_text = is_showing_placeholder_text
+        if title is not None:
+            self.title = title
+        if date_storage_format is not None:
+            self.date_storage_format = date_storage_format
+        if building_block_gallery is not None:
+            self.building_block_gallery = building_block_gallery
+        if building_block_category is not None:
+            self.building_block_category = building_block_category
+        if multiline is not None:
+            self.multiline = multiline
+        if color is not None:
+            self.color = color
+        if style_name is not None:
+            self.style_name = style_name
+        if calendar_type is not None:
+            self.calendar_type = calendar_type
         if is_temporary is not None:
             self.is_temporary = is_temporary
         if level is not None:
             self.level = level
-        if list_items is not None:
-            self.list_items = list_items
+        if sdt_type is not None:
+            self.sdt_type = sdt_type
+        if placeholder_name is not None:
+            self.placeholder_name = placeholder_name
         if lock_content_control is not None:
             self.lock_content_control = lock_content_control
         if lock_contents is not None:
             self.lock_contents = lock_contents
-        if multiline is not None:
-            self.multiline = multiline
-        if placeholder_name is not None:
-            self.placeholder_name = placeholder_name
-        if sdt_type is not None:
-            self.sdt_type = sdt_type
-        if style_name is not None:
-            self.style_name = style_name
+        if is_showing_placeholder_text is not None:
+            self.is_showing_placeholder_text = is_showing_placeholder_text
         if tag is not None:
             self.tag = tag
-        if title is not None:
-            self.title = title
+        if id is not None:
+            self.id = id
         if word_open_xml is not None:
             self.word_open_xml = word_open_xml
 
     @property
     def link(self):
         """Gets the link of this StructuredDocumentTag.  # noqa: E501
 
@@ -224,14 +224,58 @@
 
         :param node_id: The node_id of this StructuredDocumentTag.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
+    def list_items(self):
+        """Gets the list_items of this StructuredDocumentTag.  # noqa: E501
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :return: The list_items of this StructuredDocumentTag.  # noqa: E501
+        :rtype: list[StructuredDocumentTagListItem]
+        """
+        return self._list_items
+
+    @list_items.setter
+    def list_items(self, list_items):
+        """Sets the list_items of this StructuredDocumentTag.
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :param list_items: The list_items of this StructuredDocumentTag.  # noqa: E501
+        :type: list[StructuredDocumentTagListItem]
+        """
+        self._list_items = list_items
+
+    @property
+    def checked(self):
+        """Gets the checked of this StructuredDocumentTag.  # noqa: E501
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :return: The checked of this StructuredDocumentTag.  # noqa: E501
+        :rtype: bool
+        """
+        return self._checked
+
+    @checked.setter
+    def checked(self, checked):
+        """Sets the checked of this StructuredDocumentTag.
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :param checked: The checked of this StructuredDocumentTag.  # noqa: E501
+        :type: bool
+        """
+        self._checked = checked
+
+    @property
     def appearance(self):
         """Gets the appearance of this StructuredDocumentTag.  # noqa: E501
 
         Gets or sets the appearance of a structured document tag.  # noqa: E501
 
         :return: The appearance of this StructuredDocumentTag.  # noqa: E501
         :rtype: str
@@ -254,270 +298,270 @@
                     "Invalid value for `appearance` ({0}), must be one of {1}"  # noqa: E501
                     .format(appearance, allowed_values))
             self._appearance = appearance
         else:
             self._appearance = allowed_values[int(appearance) if six.PY3 else long(appearance)]
 
     @property
-    def building_block_category(self):
-        """Gets the building_block_category of this StructuredDocumentTag.  # noqa: E501
+    def date_display_locale(self):
+        """Gets the date_display_locale of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :return: The building_block_category of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
+        :return: The date_display_locale of this StructuredDocumentTag.  # noqa: E501
+        :rtype: int
         """
-        return self._building_block_category
+        return self._date_display_locale
 
-    @building_block_category.setter
-    def building_block_category(self, building_block_category):
-        """Sets the building_block_category of this StructuredDocumentTag.
+    @date_display_locale.setter
+    def date_display_locale(self, date_display_locale):
+        """Sets the date_display_locale of this StructuredDocumentTag.
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :param building_block_category: The building_block_category of this StructuredDocumentTag.  # noqa: E501
-        :type: str
+        :param date_display_locale: The date_display_locale of this StructuredDocumentTag.  # noqa: E501
+        :type: int
         """
-        self._building_block_category = building_block_category
+        self._date_display_locale = date_display_locale
 
     @property
-    def building_block_gallery(self):
-        """Gets the building_block_gallery of this StructuredDocumentTag.  # noqa: E501
+    def date_display_format(self):
+        """Gets the date_display_format of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :return: The building_block_gallery of this StructuredDocumentTag.  # noqa: E501
+        :return: The date_display_format of this StructuredDocumentTag.  # noqa: E501
         :rtype: str
         """
-        return self._building_block_gallery
+        return self._date_display_format
 
-    @building_block_gallery.setter
-    def building_block_gallery(self, building_block_gallery):
-        """Sets the building_block_gallery of this StructuredDocumentTag.
+    @date_display_format.setter
+    def date_display_format(self, date_display_format):
+        """Sets the date_display_format of this StructuredDocumentTag.
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTag.  # noqa: E501
+        :param date_display_format: The date_display_format of this StructuredDocumentTag.  # noqa: E501
         :type: str
         """
-        self._building_block_gallery = building_block_gallery
+        self._date_display_format = date_display_format
 
     @property
-    def calendar_type(self):
-        """Gets the calendar_type of this StructuredDocumentTag.  # noqa: E501
+    def full_date(self):
+        """Gets the full_date of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :return: The calendar_type of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
+        :return: The full_date of this StructuredDocumentTag.  # noqa: E501
+        :rtype: datetime
         """
-        return self._calendar_type
+        return self._full_date
 
-    @calendar_type.setter
-    def calendar_type(self, calendar_type):
-        """Sets the calendar_type of this StructuredDocumentTag.
+    @full_date.setter
+    def full_date(self, full_date):
+        """Sets the full_date of this StructuredDocumentTag.
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :param calendar_type: The calendar_type of this StructuredDocumentTag.  # noqa: E501
-        :type: str
+        :param full_date: The full_date of this StructuredDocumentTag.  # noqa: E501
+        :type: datetime
         """
-        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
-        if not calendar_type.isdigit():
-            if calendar_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(calendar_type, allowed_values))
-            self._calendar_type = calendar_type
-        else:
-            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
+        self._full_date = full_date
 
     @property
-    def checked(self):
-        """Gets the checked of this StructuredDocumentTag.  # noqa: E501
+    def title(self):
+        """Gets the title of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :return: The checked of this StructuredDocumentTag.  # noqa: E501
-        :rtype: bool
+        :return: The title of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._checked
+        return self._title
 
-    @checked.setter
-    def checked(self, checked):
-        """Sets the checked of this StructuredDocumentTag.
+    @title.setter
+    def title(self, title):
+        """Sets the title of this StructuredDocumentTag.
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :param checked: The checked of this StructuredDocumentTag.  # noqa: E501
-        :type: bool
+        :param title: The title of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._checked = checked
+        self._title = title
 
     @property
-    def color(self):
-        """Gets the color of this StructuredDocumentTag.  # noqa: E501
+    def date_storage_format(self):
+        """Gets the date_storage_format of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :return: The color of this StructuredDocumentTag.  # noqa: E501
+        :return: The date_storage_format of this StructuredDocumentTag.  # noqa: E501
         :rtype: str
         """
-        return self._color
+        return self._date_storage_format
 
-    @color.setter
-    def color(self, color):
-        """Sets the color of this StructuredDocumentTag.
+    @date_storage_format.setter
+    def date_storage_format(self, date_storage_format):
+        """Sets the date_storage_format of this StructuredDocumentTag.
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :param color: The color of this StructuredDocumentTag.  # noqa: E501
+        :param date_storage_format: The date_storage_format of this StructuredDocumentTag.  # noqa: E501
         :type: str
         """
-        self._color = color
+        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
+        if not date_storage_format.isdigit():
+            if date_storage_format not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
+                    .format(date_storage_format, allowed_values))
+            self._date_storage_format = date_storage_format
+        else:
+            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
 
     @property
-    def date_display_format(self):
-        """Gets the date_display_format of this StructuredDocumentTag.  # noqa: E501
+    def building_block_gallery(self):
+        """Gets the building_block_gallery of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :return: The date_display_format of this StructuredDocumentTag.  # noqa: E501
+        :return: The building_block_gallery of this StructuredDocumentTag.  # noqa: E501
         :rtype: str
         """
-        return self._date_display_format
+        return self._building_block_gallery
 
-    @date_display_format.setter
-    def date_display_format(self, date_display_format):
-        """Sets the date_display_format of this StructuredDocumentTag.
+    @building_block_gallery.setter
+    def building_block_gallery(self, building_block_gallery):
+        """Sets the building_block_gallery of this StructuredDocumentTag.
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :param date_display_format: The date_display_format of this StructuredDocumentTag.  # noqa: E501
+        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTag.  # noqa: E501
         :type: str
         """
-        self._date_display_format = date_display_format
+        self._building_block_gallery = building_block_gallery
 
     @property
-    def date_display_locale(self):
-        """Gets the date_display_locale of this StructuredDocumentTag.  # noqa: E501
+    def building_block_category(self):
+        """Gets the building_block_category of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :return: The date_display_locale of this StructuredDocumentTag.  # noqa: E501
-        :rtype: int
+        :return: The building_block_category of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._date_display_locale
+        return self._building_block_category
 
-    @date_display_locale.setter
-    def date_display_locale(self, date_display_locale):
-        """Sets the date_display_locale of this StructuredDocumentTag.
+    @building_block_category.setter
+    def building_block_category(self, building_block_category):
+        """Sets the building_block_category of this StructuredDocumentTag.
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :param date_display_locale: The date_display_locale of this StructuredDocumentTag.  # noqa: E501
-        :type: int
+        :param building_block_category: The building_block_category of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._date_display_locale = date_display_locale
+        self._building_block_category = building_block_category
 
     @property
-    def date_storage_format(self):
-        """Gets the date_storage_format of this StructuredDocumentTag.  # noqa: E501
+    def multiline(self):
+        """Gets the multiline of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :return: The date_storage_format of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
+        :return: The multiline of this StructuredDocumentTag.  # noqa: E501
+        :rtype: bool
         """
-        return self._date_storage_format
+        return self._multiline
 
-    @date_storage_format.setter
-    def date_storage_format(self, date_storage_format):
-        """Sets the date_storage_format of this StructuredDocumentTag.
+    @multiline.setter
+    def multiline(self, multiline):
+        """Sets the multiline of this StructuredDocumentTag.
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :param date_storage_format: The date_storage_format of this StructuredDocumentTag.  # noqa: E501
-        :type: str
+        :param multiline: The multiline of this StructuredDocumentTag.  # noqa: E501
+        :type: bool
         """
-        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
-        if not date_storage_format.isdigit():
-            if date_storage_format not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
-                    .format(date_storage_format, allowed_values))
-            self._date_storage_format = date_storage_format
-        else:
-            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
+        self._multiline = multiline
 
     @property
-    def full_date(self):
-        """Gets the full_date of this StructuredDocumentTag.  # noqa: E501
+    def color(self):
+        """Gets the color of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :return: The full_date of this StructuredDocumentTag.  # noqa: E501
-        :rtype: datetime
+        :return: The color of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._full_date
+        return self._color
 
-    @full_date.setter
-    def full_date(self, full_date):
-        """Sets the full_date of this StructuredDocumentTag.
+    @color.setter
+    def color(self, color):
+        """Sets the color of this StructuredDocumentTag.
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :param full_date: The full_date of this StructuredDocumentTag.  # noqa: E501
-        :type: datetime
+        :param color: The color of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._full_date = full_date
+        self._color = color
 
     @property
-    def id(self):
-        """Gets the id of this StructuredDocumentTag.  # noqa: E501
+    def style_name(self):
+        """Gets the style_name of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :return: The id of this StructuredDocumentTag.  # noqa: E501
-        :rtype: int
+        :return: The style_name of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._id
+        return self._style_name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this StructuredDocumentTag.
+    @style_name.setter
+    def style_name(self, style_name):
+        """Sets the style_name of this StructuredDocumentTag.
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :param id: The id of this StructuredDocumentTag.  # noqa: E501
-        :type: int
+        :param style_name: The style_name of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._id = id
+        self._style_name = style_name
 
     @property
-    def is_showing_placeholder_text(self):
-        """Gets the is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
+    def calendar_type(self):
+        """Gets the calendar_type of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :return: The is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
-        :rtype: bool
+        :return: The calendar_type of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._is_showing_placeholder_text
+        return self._calendar_type
 
-    @is_showing_placeholder_text.setter
-    def is_showing_placeholder_text(self, is_showing_placeholder_text):
-        """Sets the is_showing_placeholder_text of this StructuredDocumentTag.
+    @calendar_type.setter
+    def calendar_type(self, calendar_type):
+        """Sets the calendar_type of this StructuredDocumentTag.
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
-        :type: bool
+        :param calendar_type: The calendar_type of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._is_showing_placeholder_text = is_showing_placeholder_text
+        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
+        if not calendar_type.isdigit():
+            if calendar_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(calendar_type, allowed_values))
+            self._calendar_type = calendar_type
+        else:
+            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
 
     @property
     def is_temporary(self):
         """Gets the is_temporary of this StructuredDocumentTag.  # noqa: E501
 
         Gets or sets a value indicating whether this SDT shall be removed from the WordProcessingML document when its contents are modified.  # noqa: E501
 
@@ -564,34 +608,64 @@
                     "Invalid value for `level` ({0}), must be one of {1}"  # noqa: E501
                     .format(level, allowed_values))
             self._level = level
         else:
             self._level = allowed_values[int(level) if six.PY3 else long(level)]
 
     @property
-    def list_items(self):
-        """Gets the list_items of this StructuredDocumentTag.  # noqa: E501
+    def sdt_type(self):
+        """Gets the sdt_type of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :return: The list_items of this StructuredDocumentTag.  # noqa: E501
-        :rtype: list[StructuredDocumentTagListItem]
+        :return: The sdt_type of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
         """
-        return self._list_items
+        return self._sdt_type
 
-    @list_items.setter
-    def list_items(self, list_items):
-        """Sets the list_items of this StructuredDocumentTag.
+    @sdt_type.setter
+    def sdt_type(self, sdt_type):
+        """Sets the sdt_type of this StructuredDocumentTag.
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :param list_items: The list_items of this StructuredDocumentTag.  # noqa: E501
-        :type: list[StructuredDocumentTagListItem]
+        :param sdt_type: The sdt_type of this StructuredDocumentTag.  # noqa: E501
+        :type: str
         """
-        self._list_items = list_items
+        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
+        if not sdt_type.isdigit():
+            if sdt_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(sdt_type, allowed_values))
+            self._sdt_type = sdt_type
+        else:
+            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
+
+    @property
+    def placeholder_name(self):
+        """Gets the placeholder_name of this StructuredDocumentTag.  # noqa: E501
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :return: The placeholder_name of this StructuredDocumentTag.  # noqa: E501
+        :rtype: str
+        """
+        return self._placeholder_name
+
+    @placeholder_name.setter
+    def placeholder_name(self, placeholder_name):
+        """Sets the placeholder_name of this StructuredDocumentTag.
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :param placeholder_name: The placeholder_name of this StructuredDocumentTag.  # noqa: E501
+        :type: str
+        """
+        self._placeholder_name = placeholder_name
 
     @property
     def lock_content_control(self):
         """Gets the lock_content_control of this StructuredDocumentTag.  # noqa: E501
 
         Gets or sets a value indicating whether, this property will prohibit a user from deleting this SDT.  # noqa: E501
 
@@ -630,108 +704,34 @@
 
         :param lock_contents: The lock_contents of this StructuredDocumentTag.  # noqa: E501
         :type: bool
         """
         self._lock_contents = lock_contents
 
     @property
-    def multiline(self):
-        """Gets the multiline of this StructuredDocumentTag.  # noqa: E501
+    def is_showing_placeholder_text(self):
+        """Gets the is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :return: The multiline of this StructuredDocumentTag.  # noqa: E501
+        :return: The is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
         :rtype: bool
         """
-        return self._multiline
+        return self._is_showing_placeholder_text
 
-    @multiline.setter
-    def multiline(self, multiline):
-        """Sets the multiline of this StructuredDocumentTag.
+    @is_showing_placeholder_text.setter
+    def is_showing_placeholder_text(self, is_showing_placeholder_text):
+        """Sets the is_showing_placeholder_text of this StructuredDocumentTag.
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :param multiline: The multiline of this StructuredDocumentTag.  # noqa: E501
+        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTag.  # noqa: E501
         :type: bool
         """
-        self._multiline = multiline
-
-    @property
-    def placeholder_name(self):
-        """Gets the placeholder_name of this StructuredDocumentTag.  # noqa: E501
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :return: The placeholder_name of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
-        """
-        return self._placeholder_name
-
-    @placeholder_name.setter
-    def placeholder_name(self, placeholder_name):
-        """Sets the placeholder_name of this StructuredDocumentTag.
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :param placeholder_name: The placeholder_name of this StructuredDocumentTag.  # noqa: E501
-        :type: str
-        """
-        self._placeholder_name = placeholder_name
-
-    @property
-    def sdt_type(self):
-        """Gets the sdt_type of this StructuredDocumentTag.  # noqa: E501
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :return: The sdt_type of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
-        """
-        return self._sdt_type
-
-    @sdt_type.setter
-    def sdt_type(self, sdt_type):
-        """Sets the sdt_type of this StructuredDocumentTag.
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :param sdt_type: The sdt_type of this StructuredDocumentTag.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
-        if not sdt_type.isdigit():
-            if sdt_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(sdt_type, allowed_values))
-            self._sdt_type = sdt_type
-        else:
-            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
-
-    @property
-    def style_name(self):
-        """Gets the style_name of this StructuredDocumentTag.  # noqa: E501
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :return: The style_name of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
-        """
-        return self._style_name
-
-    @style_name.setter
-    def style_name(self, style_name):
-        """Sets the style_name of this StructuredDocumentTag.
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :param style_name: The style_name of this StructuredDocumentTag.  # noqa: E501
-        :type: str
-        """
-        self._style_name = style_name
+        self._is_showing_placeholder_text = is_showing_placeholder_text
 
     @property
     def tag(self):
         """Gets the tag of this StructuredDocumentTag.  # noqa: E501
 
         Gets or sets a tag associated with the current SDT node. Can not be null.  # noqa: E501
 
@@ -748,34 +748,34 @@
 
         :param tag: The tag of this StructuredDocumentTag.  # noqa: E501
         :type: str
         """
         self._tag = tag
 
     @property
-    def title(self):
-        """Gets the title of this StructuredDocumentTag.  # noqa: E501
+    def id(self):
+        """Gets the id of this StructuredDocumentTag.  # noqa: E501
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :return: The title of this StructuredDocumentTag.  # noqa: E501
-        :rtype: str
+        :return: The id of this StructuredDocumentTag.  # noqa: E501
+        :rtype: int
         """
-        return self._title
+        return self._id
 
-    @title.setter
-    def title(self, title):
-        """Sets the title of this StructuredDocumentTag.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StructuredDocumentTag.
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :param title: The title of this StructuredDocumentTag.  # noqa: E501
-        :type: str
+        :param id: The id of this StructuredDocumentTag.  # noqa: E501
+        :type: int
         """
-        self._title = title
+        self._id = id
 
     @property
     def word_open_xml(self):
         """Gets the word_open_xml of this StructuredDocumentTag.  # noqa: E501
 
         Gets a string that represents the XML contained within the node in the Aspose.Words.SaveFormat.FlatOpc format.  # noqa: E501
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/font_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/font_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_insert_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/range_document_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/range_document_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comment_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/file_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/file_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/node_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/node_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/protection_data_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,150 +40,150 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'appearance': 'str',
-        'building_block_category': 'str',
-        'building_block_gallery': 'str',
-        'calendar_type': 'str',
+        'list_items': 'list[StructuredDocumentTagListItem]',
         'checked': 'bool',
-        'color': 'str',
-        'date_display_format': 'str',
+        'appearance': 'str',
         'date_display_locale': 'int',
-        'date_storage_format': 'str',
+        'date_display_format': 'str',
         'full_date': 'datetime',
-        'id': 'int',
-        'is_showing_placeholder_text': 'bool',
+        'title': 'str',
+        'date_storage_format': 'str',
+        'building_block_gallery': 'str',
+        'building_block_category': 'str',
+        'multiline': 'bool',
+        'color': 'str',
+        'style_name': 'str',
+        'calendar_type': 'str',
         'is_temporary': 'bool',
         'level': 'str',
-        'list_items': 'list[StructuredDocumentTagListItem]',
+        'sdt_type': 'str',
+        'placeholder_name': 'str',
         'lock_content_control': 'bool',
         'lock_contents': 'bool',
-        'multiline': 'bool',
-        'placeholder_name': 'str',
-        'sdt_type': 'str',
-        'style_name': 'str',
+        'is_showing_placeholder_text': 'bool',
         'tag': 'str',
-        'title': 'str',
+        'id': 'int',
         'word_open_xml': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'appearance': 'Appearance',
-        'building_block_category': 'BuildingBlockCategory',
-        'building_block_gallery': 'BuildingBlockGallery',
-        'calendar_type': 'CalendarType',
+        'list_items': 'ListItems',
         'checked': 'Checked',
-        'color': 'Color',
-        'date_display_format': 'DateDisplayFormat',
+        'appearance': 'Appearance',
         'date_display_locale': 'DateDisplayLocale',
-        'date_storage_format': 'DateStorageFormat',
+        'date_display_format': 'DateDisplayFormat',
         'full_date': 'FullDate',
-        'id': 'Id',
-        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
+        'title': 'Title',
+        'date_storage_format': 'DateStorageFormat',
+        'building_block_gallery': 'BuildingBlockGallery',
+        'building_block_category': 'BuildingBlockCategory',
+        'multiline': 'Multiline',
+        'color': 'Color',
+        'style_name': 'StyleName',
+        'calendar_type': 'CalendarType',
         'is_temporary': 'IsTemporary',
         'level': 'Level',
-        'list_items': 'ListItems',
+        'sdt_type': 'SdtType',
+        'placeholder_name': 'PlaceholderName',
         'lock_content_control': 'LockContentControl',
         'lock_contents': 'LockContents',
-        'multiline': 'Multiline',
-        'placeholder_name': 'PlaceholderName',
-        'sdt_type': 'SdtType',
-        'style_name': 'StyleName',
+        'is_showing_placeholder_text': 'IsShowingPlaceholderText',
         'tag': 'Tag',
-        'title': 'Title',
+        'id': 'Id',
         'word_open_xml': 'WordOpenXML'
     }
 
-    def __init__(self, link=None, node_id=None, appearance=None, building_block_category=None, building_block_gallery=None, calendar_type=None, checked=None, color=None, date_display_format=None, date_display_locale=None, date_storage_format=None, full_date=None, id=None, is_showing_placeholder_text=None, is_temporary=None, level=None, list_items=None, lock_content_control=None, lock_contents=None, multiline=None, placeholder_name=None, sdt_type=None, style_name=None, tag=None, title=None, word_open_xml=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, list_items=None, checked=None, appearance=None, date_display_locale=None, date_display_format=None, full_date=None, title=None, date_storage_format=None, building_block_gallery=None, building_block_category=None, multiline=None, color=None, style_name=None, calendar_type=None, is_temporary=None, level=None, sdt_type=None, placeholder_name=None, lock_content_control=None, lock_contents=None, is_showing_placeholder_text=None, tag=None, id=None, word_open_xml=None):  # noqa: E501
         """StructuredDocumentTagInsert - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._appearance = None
-        self._building_block_category = None
-        self._building_block_gallery = None
-        self._calendar_type = None
+        self._list_items = None
         self._checked = None
-        self._color = None
-        self._date_display_format = None
+        self._appearance = None
         self._date_display_locale = None
-        self._date_storage_format = None
+        self._date_display_format = None
         self._full_date = None
-        self._id = None
-        self._is_showing_placeholder_text = None
+        self._title = None
+        self._date_storage_format = None
+        self._building_block_gallery = None
+        self._building_block_category = None
+        self._multiline = None
+        self._color = None
+        self._style_name = None
+        self._calendar_type = None
         self._is_temporary = None
         self._level = None
-        self._list_items = None
+        self._sdt_type = None
+        self._placeholder_name = None
         self._lock_content_control = None
         self._lock_contents = None
-        self._multiline = None
-        self._placeholder_name = None
-        self._sdt_type = None
-        self._style_name = None
+        self._is_showing_placeholder_text = None
         self._tag = None
-        self._title = None
+        self._id = None
         self._word_open_xml = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if appearance is not None:
-            self.appearance = appearance
-        if building_block_category is not None:
-            self.building_block_category = building_block_category
-        if building_block_gallery is not None:
-            self.building_block_gallery = building_block_gallery
-        if calendar_type is not None:
-            self.calendar_type = calendar_type
+        if list_items is not None:
+            self.list_items = list_items
         if checked is not None:
             self.checked = checked
-        if color is not None:
-            self.color = color
-        if date_display_format is not None:
-            self.date_display_format = date_display_format
+        if appearance is not None:
+            self.appearance = appearance
         if date_display_locale is not None:
             self.date_display_locale = date_display_locale
-        if date_storage_format is not None:
-            self.date_storage_format = date_storage_format
+        if date_display_format is not None:
+            self.date_display_format = date_display_format
         if full_date is not None:
             self.full_date = full_date
-        if id is not None:
-            self.id = id
-        if is_showing_placeholder_text is not None:
-            self.is_showing_placeholder_text = is_showing_placeholder_text
+        if title is not None:
+            self.title = title
+        if date_storage_format is not None:
+            self.date_storage_format = date_storage_format
+        if building_block_gallery is not None:
+            self.building_block_gallery = building_block_gallery
+        if building_block_category is not None:
+            self.building_block_category = building_block_category
+        if multiline is not None:
+            self.multiline = multiline
+        if color is not None:
+            self.color = color
+        if style_name is not None:
+            self.style_name = style_name
+        if calendar_type is not None:
+            self.calendar_type = calendar_type
         if is_temporary is not None:
             self.is_temporary = is_temporary
         if level is not None:
             self.level = level
-        if list_items is not None:
-            self.list_items = list_items
+        if sdt_type is not None:
+            self.sdt_type = sdt_type
+        if placeholder_name is not None:
+            self.placeholder_name = placeholder_name
         if lock_content_control is not None:
             self.lock_content_control = lock_content_control
         if lock_contents is not None:
             self.lock_contents = lock_contents
-        if multiline is not None:
-            self.multiline = multiline
-        if placeholder_name is not None:
-            self.placeholder_name = placeholder_name
-        if sdt_type is not None:
-            self.sdt_type = sdt_type
-        if style_name is not None:
-            self.style_name = style_name
+        if is_showing_placeholder_text is not None:
+            self.is_showing_placeholder_text = is_showing_placeholder_text
         if tag is not None:
             self.tag = tag
-        if title is not None:
-            self.title = title
+        if id is not None:
+            self.id = id
         if word_open_xml is not None:
             self.word_open_xml = word_open_xml
 
     @property
     def link(self):
         """Gets the link of this StructuredDocumentTagInsert.  # noqa: E501
 
@@ -224,14 +224,58 @@
 
         :param node_id: The node_id of this StructuredDocumentTagInsert.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
+    def list_items(self):
+        """Gets the list_items of this StructuredDocumentTagInsert.  # noqa: E501
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :return: The list_items of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: list[StructuredDocumentTagListItem]
+        """
+        return self._list_items
+
+    @list_items.setter
+    def list_items(self, list_items):
+        """Sets the list_items of this StructuredDocumentTagInsert.
+
+        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+
+        :param list_items: The list_items of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: list[StructuredDocumentTagListItem]
+        """
+        self._list_items = list_items
+
+    @property
+    def checked(self):
+        """Gets the checked of this StructuredDocumentTagInsert.  # noqa: E501
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :return: The checked of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: bool
+        """
+        return self._checked
+
+    @checked.setter
+    def checked(self, checked):
+        """Sets the checked of this StructuredDocumentTagInsert.
+
+        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+
+        :param checked: The checked of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: bool
+        """
+        self._checked = checked
+
+    @property
     def appearance(self):
         """Gets the appearance of this StructuredDocumentTagInsert.  # noqa: E501
 
         Gets or sets the appearance of a structured document tag.  # noqa: E501
 
         :return: The appearance of this StructuredDocumentTagInsert.  # noqa: E501
         :rtype: str
@@ -254,270 +298,270 @@
                     "Invalid value for `appearance` ({0}), must be one of {1}"  # noqa: E501
                     .format(appearance, allowed_values))
             self._appearance = appearance
         else:
             self._appearance = allowed_values[int(appearance) if six.PY3 else long(appearance)]
 
     @property
-    def building_block_category(self):
-        """Gets the building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
+    def date_display_locale(self):
+        """Gets the date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :return: The building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
+        :return: The date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: int
         """
-        return self._building_block_category
+        return self._date_display_locale
 
-    @building_block_category.setter
-    def building_block_category(self, building_block_category):
-        """Sets the building_block_category of this StructuredDocumentTagInsert.
+    @date_display_locale.setter
+    def date_display_locale(self, date_display_locale):
+        """Sets the date_display_locale of this StructuredDocumentTagInsert.
 
-        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
+        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
 
-        :param building_block_category: The building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
+        :param date_display_locale: The date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: int
         """
-        self._building_block_category = building_block_category
+        self._date_display_locale = date_display_locale
 
     @property
-    def building_block_gallery(self):
-        """Gets the building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
+    def date_display_format(self):
+        """Gets the date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :return: The building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
+        :return: The date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
         :rtype: str
         """
-        return self._building_block_gallery
+        return self._date_display_format
 
-    @building_block_gallery.setter
-    def building_block_gallery(self, building_block_gallery):
-        """Sets the building_block_gallery of this StructuredDocumentTagInsert.
+    @date_display_format.setter
+    def date_display_format(self, date_display_format):
+        """Sets the date_display_format of this StructuredDocumentTagInsert.
 
-        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
+        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
 
-        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
+        :param date_display_format: The date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
         :type: str
         """
-        self._building_block_gallery = building_block_gallery
+        self._date_display_format = date_display_format
 
     @property
-    def calendar_type(self):
-        """Gets the calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
+    def full_date(self):
+        """Gets the full_date of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :return: The calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
+        :return: The full_date of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: datetime
         """
-        return self._calendar_type
+        return self._full_date
 
-    @calendar_type.setter
-    def calendar_type(self, calendar_type):
-        """Sets the calendar_type of this StructuredDocumentTagInsert.
+    @full_date.setter
+    def full_date(self, full_date):
+        """Sets the full_date of this StructuredDocumentTagInsert.
 
-        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
+        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
 
-        :param calendar_type: The calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
+        :param full_date: The full_date of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: datetime
         """
-        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
-        if not calendar_type.isdigit():
-            if calendar_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(calendar_type, allowed_values))
-            self._calendar_type = calendar_type
-        else:
-            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
+        self._full_date = full_date
 
     @property
-    def checked(self):
-        """Gets the checked of this StructuredDocumentTagInsert.  # noqa: E501
+    def title(self):
+        """Gets the title of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :return: The checked of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: bool
+        :return: The title of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._checked
+        return self._title
 
-    @checked.setter
-    def checked(self, checked):
-        """Sets the checked of this StructuredDocumentTagInsert.
+    @title.setter
+    def title(self, title):
+        """Sets the title of this StructuredDocumentTagInsert.
 
-        Gets or sets a value indicating whether current state of the Checkbox SDT. Default value for this property.  # noqa: E501
+        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
 
-        :param checked: The checked of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: bool
+        :param title: The title of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._checked = checked
+        self._title = title
 
     @property
-    def color(self):
-        """Gets the color of this StructuredDocumentTagInsert.  # noqa: E501
+    def date_storage_format(self):
+        """Gets the date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :return: The color of this StructuredDocumentTagInsert.  # noqa: E501
+        :return: The date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
         :rtype: str
         """
-        return self._color
+        return self._date_storage_format
 
-    @color.setter
-    def color(self, color):
-        """Sets the color of this StructuredDocumentTagInsert.
+    @date_storage_format.setter
+    def date_storage_format(self, date_storage_format):
+        """Sets the date_storage_format of this StructuredDocumentTagInsert.
 
-        Gets or sets the color of the structured document tag.  # noqa: E501
+        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
 
-        :param color: The color of this StructuredDocumentTagInsert.  # noqa: E501
+        :param date_storage_format: The date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
         :type: str
         """
-        self._color = color
+        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
+        if not date_storage_format.isdigit():
+            if date_storage_format not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
+                    .format(date_storage_format, allowed_values))
+            self._date_storage_format = date_storage_format
+        else:
+            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
 
     @property
-    def date_display_format(self):
-        """Gets the date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
+    def building_block_gallery(self):
+        """Gets the building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :return: The date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
+        :return: The building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
         :rtype: str
         """
-        return self._date_display_format
+        return self._building_block_gallery
 
-    @date_display_format.setter
-    def date_display_format(self, date_display_format):
-        """Sets the date_display_format of this StructuredDocumentTagInsert.
+    @building_block_gallery.setter
+    def building_block_gallery(self, building_block_gallery):
+        """Sets the building_block_gallery of this StructuredDocumentTagInsert.
 
-        Gets or sets String that represents the format in which dates are displayed. Can not be null. The dates for English (U.S.) is "mm/dd/yyyy".  # noqa: E501
+        Gets or sets type of building block for this SDT. Can not be null.  # noqa: E501
 
-        :param date_display_format: The date_display_format of this StructuredDocumentTagInsert.  # noqa: E501
+        :param building_block_gallery: The building_block_gallery of this StructuredDocumentTagInsert.  # noqa: E501
         :type: str
         """
-        self._date_display_format = date_display_format
+        self._building_block_gallery = building_block_gallery
 
     @property
-    def date_display_locale(self):
-        """Gets the date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
+    def building_block_category(self):
+        """Gets the building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :return: The date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: int
+        :return: The building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._date_display_locale
+        return self._building_block_category
 
-    @date_display_locale.setter
-    def date_display_locale(self, date_display_locale):
-        """Sets the date_display_locale of this StructuredDocumentTagInsert.
+    @building_block_category.setter
+    def building_block_category(self, building_block_category):
+        """Sets the building_block_category of this StructuredDocumentTagInsert.
 
-        Gets or sets the language format for the date displayed in this SDT.  # noqa: E501
+        Gets or sets category of building block for this SDT node. Can not be null.  # noqa: E501
 
-        :param date_display_locale: The date_display_locale of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: int
+        :param building_block_category: The building_block_category of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._date_display_locale = date_display_locale
+        self._building_block_category = building_block_category
 
     @property
-    def date_storage_format(self):
-        """Gets the date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
+    def multiline(self):
+        """Gets the multiline of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :return: The date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
+        :return: The multiline of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: bool
         """
-        return self._date_storage_format
+        return self._multiline
 
-    @date_storage_format.setter
-    def date_storage_format(self, date_storage_format):
-        """Sets the date_storage_format of this StructuredDocumentTagInsert.
+    @multiline.setter
+    def multiline(self, multiline):
+        """Sets the multiline of this StructuredDocumentTagInsert.
 
-        Gets or sets format in which the date for a date SDT is stored when the SDT is bound to an XML node in the document's data store. Default value is Aspose.Words.Markup.SdtDateStorageFormat.DateTime.  # noqa: E501
+        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
 
-        :param date_storage_format: The date_storage_format of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
+        :param multiline: The multiline of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: bool
         """
-        allowed_values = ["Date", "DateTime", "Default", "Text"]  # noqa: E501
-        if not date_storage_format.isdigit():
-            if date_storage_format not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `date_storage_format` ({0}), must be one of {1}"  # noqa: E501
-                    .format(date_storage_format, allowed_values))
-            self._date_storage_format = date_storage_format
-        else:
-            self._date_storage_format = allowed_values[int(date_storage_format) if six.PY3 else long(date_storage_format)]
+        self._multiline = multiline
 
     @property
-    def full_date(self):
-        """Gets the full_date of this StructuredDocumentTagInsert.  # noqa: E501
+    def color(self):
+        """Gets the color of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :return: The full_date of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: datetime
+        :return: The color of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._full_date
+        return self._color
 
-    @full_date.setter
-    def full_date(self, full_date):
-        """Sets the full_date of this StructuredDocumentTagInsert.
+    @color.setter
+    def color(self, color):
+        """Sets the color of this StructuredDocumentTagInsert.
 
-        Gets or sets the full date and time last entered into this SDT.  # noqa: E501
+        Gets or sets the color of the structured document tag.  # noqa: E501
 
-        :param full_date: The full_date of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: datetime
+        :param color: The color of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._full_date = full_date
+        self._color = color
 
     @property
-    def id(self):
-        """Gets the id of this StructuredDocumentTagInsert.  # noqa: E501
+    def style_name(self):
+        """Gets the style_name of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :return: The id of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: int
+        :return: The style_name of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._id
+        return self._style_name
 
-    @id.setter
-    def id(self, id):
-        """Sets the id of this StructuredDocumentTagInsert.
+    @style_name.setter
+    def style_name(self, style_name):
+        """Sets the style_name of this StructuredDocumentTagInsert.
 
-        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
+        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
 
-        :param id: The id of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: int
+        :param style_name: The style_name of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._id = id
+        self._style_name = style_name
 
     @property
-    def is_showing_placeholder_text(self):
-        """Gets the is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
+    def calendar_type(self):
+        """Gets the calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :return: The is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: bool
+        :return: The calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._is_showing_placeholder_text
+        return self._calendar_type
 
-    @is_showing_placeholder_text.setter
-    def is_showing_placeholder_text(self, is_showing_placeholder_text):
-        """Sets the is_showing_placeholder_text of this StructuredDocumentTagInsert.
+    @calendar_type.setter
+    def calendar_type(self, calendar_type):
+        """Sets the calendar_type of this StructuredDocumentTagInsert.
 
-        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
+        Gets or sets the type of calendar for this SDT. Default is Aspose.Words.Markup.SdtCalendarType.Default.  # noqa: E501
 
-        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: bool
+        :param calendar_type: The calendar_type of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._is_showing_placeholder_text = is_showing_placeholder_text
+        allowed_values = ["Default", "Gregorian", "GregorianArabic", "GregorianMeFrench", "GregorianUs", "GregorianXlitEnglish", "GregorianXlitFrench", "Hebrew", "Hijri", "Japan", "Korea", "None", "Saka", "Taiwan", "Thai"]  # noqa: E501
+        if not calendar_type.isdigit():
+            if calendar_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `calendar_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(calendar_type, allowed_values))
+            self._calendar_type = calendar_type
+        else:
+            self._calendar_type = allowed_values[int(calendar_type) if six.PY3 else long(calendar_type)]
 
     @property
     def is_temporary(self):
         """Gets the is_temporary of this StructuredDocumentTagInsert.  # noqa: E501
 
         Gets or sets a value indicating whether this SDT shall be removed from the WordProcessingML document when its contents are modified.  # noqa: E501
 
@@ -564,34 +608,64 @@
                     "Invalid value for `level` ({0}), must be one of {1}"  # noqa: E501
                     .format(level, allowed_values))
             self._level = level
         else:
             self._level = allowed_values[int(level) if six.PY3 else long(level)]
 
     @property
-    def list_items(self):
-        """Gets the list_items of this StructuredDocumentTagInsert.  # noqa: E501
+    def sdt_type(self):
+        """Gets the sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :return: The list_items of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: list[StructuredDocumentTagListItem]
+        :return: The sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
         """
-        return self._list_items
+        return self._sdt_type
 
-    @list_items.setter
-    def list_items(self, list_items):
-        """Sets the list_items of this StructuredDocumentTagInsert.
+    @sdt_type.setter
+    def sdt_type(self, sdt_type):
+        """Sets the sdt_type of this StructuredDocumentTagInsert.
 
-        Gets or sets Aspose.Words.Markup.SdtListItemCollection associated with this SDT.  # noqa: E501
+        Gets or sets type of this Structured document tag.  # noqa: E501
 
-        :param list_items: The list_items of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: list[StructuredDocumentTagListItem]
+        :param sdt_type: The sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
         """
-        self._list_items = list_items
+        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
+        if not sdt_type.isdigit():
+            if sdt_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(sdt_type, allowed_values))
+            self._sdt_type = sdt_type
+        else:
+            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
+
+    @property
+    def placeholder_name(self):
+        """Gets the placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :return: The placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: str
+        """
+        return self._placeholder_name
+
+    @placeholder_name.setter
+    def placeholder_name(self, placeholder_name):
+        """Sets the placeholder_name of this StructuredDocumentTagInsert.
+
+        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
+
+        :param placeholder_name: The placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: str
+        """
+        self._placeholder_name = placeholder_name
 
     @property
     def lock_content_control(self):
         """Gets the lock_content_control of this StructuredDocumentTagInsert.  # noqa: E501
 
         Gets or sets a value indicating whether, this property will prohibit a user from deleting this SDT.  # noqa: E501
 
@@ -630,108 +704,34 @@
 
         :param lock_contents: The lock_contents of this StructuredDocumentTagInsert.  # noqa: E501
         :type: bool
         """
         self._lock_contents = lock_contents
 
     @property
-    def multiline(self):
-        """Gets the multiline of this StructuredDocumentTagInsert.  # noqa: E501
+    def is_showing_placeholder_text(self):
+        """Gets the is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :return: The multiline of this StructuredDocumentTagInsert.  # noqa: E501
+        :return: The is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
         :rtype: bool
         """
-        return self._multiline
+        return self._is_showing_placeholder_text
 
-    @multiline.setter
-    def multiline(self, multiline):
-        """Sets the multiline of this StructuredDocumentTagInsert.
+    @is_showing_placeholder_text.setter
+    def is_showing_placeholder_text(self, is_showing_placeholder_text):
+        """Sets the is_showing_placeholder_text of this StructuredDocumentTagInsert.
 
-        Gets or sets a value indicating whether this SDT allows multiple lines of text.  # noqa: E501
+        Gets or sets a value indicating whether the content of this SDT shall be interpreted to contain placeholder text (as opposed to regular text contents within the SDT). If set to true, this state shall be resumed (showing placeholder text) upon opening his document.  # noqa: E501
 
-        :param multiline: The multiline of this StructuredDocumentTagInsert.  # noqa: E501
+        :param is_showing_placeholder_text: The is_showing_placeholder_text of this StructuredDocumentTagInsert.  # noqa: E501
         :type: bool
         """
-        self._multiline = multiline
-
-    @property
-    def placeholder_name(self):
-        """Gets the placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :return: The placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
-        """
-        return self._placeholder_name
-
-    @placeholder_name.setter
-    def placeholder_name(self, placeholder_name):
-        """Sets the placeholder_name of this StructuredDocumentTagInsert.
-
-        Gets or sets Name of the Aspose.Words.BuildingBlocks.BuildingBlock containing placeholder text. Aspose.Words.BuildingBlocks.BuildingBlock with this name Aspose.Words.BuildingBlocks.BuildingBlock.Name has to be present in the Aspose.Words.Document.GlossaryDocument otherwise System.InvalidOperationException will occur.  # noqa: E501
-
-        :param placeholder_name: The placeholder_name of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
-        """
-        self._placeholder_name = placeholder_name
-
-    @property
-    def sdt_type(self):
-        """Gets the sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :return: The sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
-        """
-        return self._sdt_type
-
-    @sdt_type.setter
-    def sdt_type(self, sdt_type):
-        """Sets the sdt_type of this StructuredDocumentTagInsert.
-
-        Gets or sets type of this Structured document tag.  # noqa: E501
-
-        :param sdt_type: The sdt_type of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["None", "Bibliography", "Citation", "Equation", "DropDownList", "ComboBox", "Date", "BuildingBlockGallery", "DocPartObj", "Group", "Picture", "RichText", "PlainText", "Checkbox", "RepeatingSection", "RepeatingSectionItem", "EntityPicker"]  # noqa: E501
-        if not sdt_type.isdigit():
-            if sdt_type not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `sdt_type` ({0}), must be one of {1}"  # noqa: E501
-                    .format(sdt_type, allowed_values))
-            self._sdt_type = sdt_type
-        else:
-            self._sdt_type = allowed_values[int(sdt_type) if six.PY3 else long(sdt_type)]
-
-    @property
-    def style_name(self):
-        """Gets the style_name of this StructuredDocumentTagInsert.  # noqa: E501
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :return: The style_name of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
-        """
-        return self._style_name
-
-    @style_name.setter
-    def style_name(self, style_name):
-        """Sets the style_name of this StructuredDocumentTagInsert.
-
-        Gets or sets the name of the style applied to the structured document tag.  # noqa: E501
-
-        :param style_name: The style_name of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
-        """
-        self._style_name = style_name
+        self._is_showing_placeholder_text = is_showing_placeholder_text
 
     @property
     def tag(self):
         """Gets the tag of this StructuredDocumentTagInsert.  # noqa: E501
 
         Gets or sets a tag associated with the current SDT node. Can not be null.  # noqa: E501
 
@@ -748,34 +748,34 @@
 
         :param tag: The tag of this StructuredDocumentTagInsert.  # noqa: E501
         :type: str
         """
         self._tag = tag
 
     @property
-    def title(self):
-        """Gets the title of this StructuredDocumentTagInsert.  # noqa: E501
+    def id(self):
+        """Gets the id of this StructuredDocumentTagInsert.  # noqa: E501
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :return: The title of this StructuredDocumentTagInsert.  # noqa: E501
-        :rtype: str
+        :return: The id of this StructuredDocumentTagInsert.  # noqa: E501
+        :rtype: int
         """
-        return self._title
+        return self._id
 
-    @title.setter
-    def title(self, title):
-        """Sets the title of this StructuredDocumentTagInsert.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this StructuredDocumentTagInsert.
 
-        Gets or sets the friendly name associated with this SDT. Can not be null.  # noqa: E501
+        Gets or sets a unique read-only persistent numerical Id for this SDT.  # noqa: E501
 
-        :param title: The title of this StructuredDocumentTagInsert.  # noqa: E501
-        :type: str
+        :param id: The id of this StructuredDocumentTagInsert.  # noqa: E501
+        :type: int
         """
-        self._title = title
+        self._id = id
 
     @property
     def word_open_xml(self):
         """Gets the word_open_xml of this StructuredDocumentTagInsert.  # noqa: E501
 
         Gets a string that represents the XML contained within the node in the Aspose.Words.SaveFormat.FlatOpc format.  # noqa: E501
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/compare_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/compare_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/load_web_document_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/load_web_document_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,56 +38,34 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'loading_document_url': 'str',
-        'save_options': 'SaveOptionsData'
+        'save_options': 'SaveOptionsData',
+        'loading_document_url': 'str'
     }
 
     attribute_map = {
-        'loading_document_url': 'LoadingDocumentUrl',
-        'save_options': 'SaveOptions'
+        'save_options': 'SaveOptions',
+        'loading_document_url': 'LoadingDocumentUrl'
     }
 
-    def __init__(self, loading_document_url=None, save_options=None):  # noqa: E501
+    def __init__(self, save_options=None, loading_document_url=None):  # noqa: E501
         """LoadWebDocumentData - a model defined in Swagger"""  # noqa: E501
 
-        self._loading_document_url = None
         self._save_options = None
+        self._loading_document_url = None
         self.discriminator = None
 
-        if loading_document_url is not None:
-            self.loading_document_url = loading_document_url
         if save_options is not None:
             self.save_options = save_options
-
-    @property
-    def loading_document_url(self):
-        """Gets the loading_document_url of this LoadWebDocumentData.  # noqa: E501
-
-        Gets or sets the web document URL.  # noqa: E501
-
-        :return: The loading_document_url of this LoadWebDocumentData.  # noqa: E501
-        :rtype: str
-        """
-        return self._loading_document_url
-
-    @loading_document_url.setter
-    def loading_document_url(self, loading_document_url):
-        """Sets the loading_document_url of this LoadWebDocumentData.
-
-        Gets or sets the web document URL.  # noqa: E501
-
-        :param loading_document_url: The loading_document_url of this LoadWebDocumentData.  # noqa: E501
-        :type: str
-        """
-        self._loading_document_url = loading_document_url
+        if loading_document_url is not None:
+            self.loading_document_url = loading_document_url
 
     @property
     def save_options(self):
         """Gets the save_options of this LoadWebDocumentData.  # noqa: E501
 
         Gets or sets the save options.  # noqa: E501
 
@@ -103,14 +81,36 @@
         Gets or sets the save options.  # noqa: E501
 
         :param save_options: The save_options of this LoadWebDocumentData.  # noqa: E501
         :type: SaveOptionsData
         """
         self._save_options = save_options
 
+    @property
+    def loading_document_url(self):
+        """Gets the loading_document_url of this LoadWebDocumentData.  # noqa: E501
+
+        Gets or sets the web document URL.  # noqa: E501
+
+        :return: The loading_document_url of this LoadWebDocumentData.  # noqa: E501
+        :rtype: str
+        """
+        return self._loading_document_url
+
+    @loading_document_url.setter
+    def loading_document_url(self, loading_document_url):
+        """Sets the loading_document_url of this LoadWebDocumentData.
+
+        Gets or sets the web document URL.  # noqa: E501
+
+        :param loading_document_url: The loading_document_url of this LoadWebDocumentData.  # noqa: E501
+        :type: str
+        """
+        self._loading_document_url = loading_document_url
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/report_build_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/report_build_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/range_text_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/range_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link_collection_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/report_engine_settings.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/report_engine_settings.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/words_api_error_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_error_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,42 +40,42 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'table_properties': 'TableProperties',
-        'table_row_list': 'list[TableRow]'
+        'table_row_list': 'list[TableRow]',
+        'table_properties': 'TableProperties'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'table_properties': 'TableProperties',
-        'table_row_list': 'TableRowList'
+        'table_row_list': 'TableRowList',
+        'table_properties': 'TableProperties'
     }
 
-    def __init__(self, link=None, node_id=None, table_properties=None, table_row_list=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, table_row_list=None, table_properties=None):  # noqa: E501
         """Table - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._table_properties = None
         self._table_row_list = None
+        self._table_properties = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if table_properties is not None:
-            self.table_properties = table_properties
         if table_row_list is not None:
             self.table_row_list = table_row_list
+        if table_properties is not None:
+            self.table_properties = table_properties
 
     @property
     def link(self):
         """Gets the link of this Table.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -114,36 +114,14 @@
 
         :param node_id: The node_id of this Table.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def table_properties(self):
-        """Gets the table_properties of this Table.  # noqa: E501
-
-        Gets or sets table properties.  # noqa: E501
-
-        :return: The table_properties of this Table.  # noqa: E501
-        :rtype: TableProperties
-        """
-        return self._table_properties
-
-    @table_properties.setter
-    def table_properties(self, table_properties):
-        """Sets the table_properties of this Table.
-
-        Gets or sets table properties.  # noqa: E501
-
-        :param table_properties: The table_properties of this Table.  # noqa: E501
-        :type: TableProperties
-        """
-        self._table_properties = table_properties
-
-    @property
     def table_row_list(self):
         """Gets the table_row_list of this Table.  # noqa: E501
 
         Gets or sets the collection of table's rows.  # noqa: E501
 
         :return: The table_row_list of this Table.  # noqa: E501
         :rtype: list[TableRow]
@@ -157,14 +135,36 @@
         Gets or sets the collection of table's rows.  # noqa: E501
 
         :param table_row_list: The table_row_list of this Table.  # noqa: E501
         :type: list[TableRow]
         """
         self._table_row_list = table_row_list
 
+    @property
+    def table_properties(self):
+        """Gets the table_properties of this Table.  # noqa: E501
+
+        Gets or sets table properties.  # noqa: E501
+
+        :return: The table_properties of this Table.  # noqa: E501
+        :rtype: TableProperties
+        """
+        return self._table_properties
+
+    @table_properties.setter
+    def table_properties(self, table_properties):
+        """Sets the table_properties of this Table.
+
+        Gets or sets table properties.  # noqa: E501
+
+        :param table_properties: The table_properties of this Table.  # noqa: E501
+        :type: TableProperties
+        """
+        self._table_properties = table_properties
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/modification_operation_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/modification_operation_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_parts_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_parts_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_checkbox.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_checkbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,92 +40,92 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'calculate_on_exit': 'bool',
+        'name': 'str',
         'enabled': 'bool',
-        'entry_macro': 'str',
-        'exit_macro': 'str',
+        'status_text': 'str',
+        'own_status': 'bool',
         'help_text': 'str',
-        'name': 'str',
         'own_help': 'bool',
-        'own_status': 'bool',
-        'status_text': 'str',
+        'calculate_on_exit': 'bool',
+        'entry_macro': 'str',
+        'exit_macro': 'str',
+        'is_check_box_exact_size': 'bool',
         'check_box_size': 'float',
-        'checked': 'bool',
-        'is_check_box_exact_size': 'bool'
+        'checked': 'bool'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'calculate_on_exit': 'CalculateOnExit',
+        'name': 'Name',
         'enabled': 'Enabled',
-        'entry_macro': 'EntryMacro',
-        'exit_macro': 'ExitMacro',
+        'status_text': 'StatusText',
+        'own_status': 'OwnStatus',
         'help_text': 'HelpText',
-        'name': 'Name',
         'own_help': 'OwnHelp',
-        'own_status': 'OwnStatus',
-        'status_text': 'StatusText',
+        'calculate_on_exit': 'CalculateOnExit',
+        'entry_macro': 'EntryMacro',
+        'exit_macro': 'ExitMacro',
+        'is_check_box_exact_size': 'IsCheckBoxExactSize',
         'check_box_size': 'CheckBoxSize',
-        'checked': 'Checked',
-        'is_check_box_exact_size': 'IsCheckBoxExactSize'
+        'checked': 'Checked'
     }
 
-    def __init__(self, link=None, node_id=None, calculate_on_exit=None, enabled=None, entry_macro=None, exit_macro=None, help_text=None, name=None, own_help=None, own_status=None, status_text=None, check_box_size=None, checked=None, is_check_box_exact_size=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, name=None, enabled=None, status_text=None, own_status=None, help_text=None, own_help=None, calculate_on_exit=None, entry_macro=None, exit_macro=None, is_check_box_exact_size=None, check_box_size=None, checked=None):  # noqa: E501
         """FormFieldCheckbox - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._calculate_on_exit = None
+        self._name = None
         self._enabled = None
-        self._entry_macro = None
-        self._exit_macro = None
+        self._status_text = None
+        self._own_status = None
         self._help_text = None
-        self._name = None
         self._own_help = None
-        self._own_status = None
-        self._status_text = None
+        self._calculate_on_exit = None
+        self._entry_macro = None
+        self._exit_macro = None
+        self._is_check_box_exact_size = None
         self._check_box_size = None
         self._checked = None
-        self._is_check_box_exact_size = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if calculate_on_exit is not None:
-            self.calculate_on_exit = calculate_on_exit
+        if name is not None:
+            self.name = name
         if enabled is not None:
             self.enabled = enabled
-        if entry_macro is not None:
-            self.entry_macro = entry_macro
-        if exit_macro is not None:
-            self.exit_macro = exit_macro
+        if status_text is not None:
+            self.status_text = status_text
+        if own_status is not None:
+            self.own_status = own_status
         if help_text is not None:
             self.help_text = help_text
-        if name is not None:
-            self.name = name
         if own_help is not None:
             self.own_help = own_help
-        if own_status is not None:
-            self.own_status = own_status
-        if status_text is not None:
-            self.status_text = status_text
+        if calculate_on_exit is not None:
+            self.calculate_on_exit = calculate_on_exit
+        if entry_macro is not None:
+            self.entry_macro = entry_macro
+        if exit_macro is not None:
+            self.exit_macro = exit_macro
+        if is_check_box_exact_size is not None:
+            self.is_check_box_exact_size = is_check_box_exact_size
         if check_box_size is not None:
             self.check_box_size = check_box_size
         if checked is not None:
             self.checked = checked
-        if is_check_box_exact_size is not None:
-            self.is_check_box_exact_size = is_check_box_exact_size
 
     @property
     def link(self):
         """Gets the link of this FormFieldCheckbox.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -164,34 +164,34 @@
 
         :param node_id: The node_id of this FormFieldCheckbox.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def calculate_on_exit(self):
-        """Gets the calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
+    def name(self):
+        """Gets the name of this FormFieldCheckbox.  # noqa: E501
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :return: The calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
-        :rtype: bool
+        :return: The name of this FormFieldCheckbox.  # noqa: E501
+        :rtype: str
         """
-        return self._calculate_on_exit
+        return self._name
 
-    @calculate_on_exit.setter
-    def calculate_on_exit(self, calculate_on_exit):
-        """Sets the calculate_on_exit of this FormFieldCheckbox.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this FormFieldCheckbox.
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :param calculate_on_exit: The calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
-        :type: bool
+        :param name: The name of this FormFieldCheckbox.  # noqa: E501
+        :type: str
         """
-        self._calculate_on_exit = calculate_on_exit
+        self._name = name
 
     @property
     def enabled(self):
         """Gets the enabled of this FormFieldCheckbox.  # noqa: E501
 
         Gets or sets a value indicating whether a form field is enabled.  # noqa: E501
 
@@ -208,56 +208,56 @@
 
         :param enabled: The enabled of this FormFieldCheckbox.  # noqa: E501
         :type: bool
         """
         self._enabled = enabled
 
     @property
-    def entry_macro(self):
-        """Gets the entry_macro of this FormFieldCheckbox.  # noqa: E501
+    def status_text(self):
+        """Gets the status_text of this FormFieldCheckbox.  # noqa: E501
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The entry_macro of this FormFieldCheckbox.  # noqa: E501
+        :return: The status_text of this FormFieldCheckbox.  # noqa: E501
         :rtype: str
         """
-        return self._entry_macro
+        return self._status_text
 
-    @entry_macro.setter
-    def entry_macro(self, entry_macro):
-        """Sets the entry_macro of this FormFieldCheckbox.
+    @status_text.setter
+    def status_text(self, status_text):
+        """Sets the status_text of this FormFieldCheckbox.
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param entry_macro: The entry_macro of this FormFieldCheckbox.  # noqa: E501
+        :param status_text: The status_text of this FormFieldCheckbox.  # noqa: E501
         :type: str
         """
-        self._entry_macro = entry_macro
+        self._status_text = status_text
 
     @property
-    def exit_macro(self):
-        """Gets the exit_macro of this FormFieldCheckbox.  # noqa: E501
+    def own_status(self):
+        """Gets the own_status of this FormFieldCheckbox.  # noqa: E501
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The exit_macro of this FormFieldCheckbox.  # noqa: E501
-        :rtype: str
+        :return: The own_status of this FormFieldCheckbox.  # noqa: E501
+        :rtype: bool
         """
-        return self._exit_macro
+        return self._own_status
 
-    @exit_macro.setter
-    def exit_macro(self, exit_macro):
-        """Sets the exit_macro of this FormFieldCheckbox.
+    @own_status.setter
+    def own_status(self, own_status):
+        """Sets the own_status of this FormFieldCheckbox.
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param exit_macro: The exit_macro of this FormFieldCheckbox.  # noqa: E501
-        :type: str
+        :param own_status: The own_status of this FormFieldCheckbox.  # noqa: E501
+        :type: bool
         """
-        self._exit_macro = exit_macro
+        self._own_status = own_status
 
     @property
     def help_text(self):
         """Gets the help_text of this FormFieldCheckbox.  # noqa: E501
 
         Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1.  # noqa: E501
 
@@ -274,36 +274,14 @@
 
         :param help_text: The help_text of this FormFieldCheckbox.  # noqa: E501
         :type: str
         """
         self._help_text = help_text
 
     @property
-    def name(self):
-        """Gets the name of this FormFieldCheckbox.  # noqa: E501
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :return: The name of this FormFieldCheckbox.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this FormFieldCheckbox.
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :param name: The name of this FormFieldCheckbox.  # noqa: E501
-        :type: str
-        """
-        self._name = name
-
-    @property
     def own_help(self):
         """Gets the own_help of this FormFieldCheckbox.  # noqa: E501
 
         Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1.  # noqa: E501
 
         :return: The own_help of this FormFieldCheckbox.  # noqa: E501
         :rtype: bool
@@ -318,56 +296,100 @@
 
         :param own_help: The own_help of this FormFieldCheckbox.  # noqa: E501
         :type: bool
         """
         self._own_help = own_help
 
     @property
-    def own_status(self):
-        """Gets the own_status of this FormFieldCheckbox.  # noqa: E501
+    def calculate_on_exit(self):
+        """Gets the calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :return: The own_status of this FormFieldCheckbox.  # noqa: E501
+        :return: The calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
         :rtype: bool
         """
-        return self._own_status
+        return self._calculate_on_exit
 
-    @own_status.setter
-    def own_status(self, own_status):
-        """Sets the own_status of this FormFieldCheckbox.
+    @calculate_on_exit.setter
+    def calculate_on_exit(self, calculate_on_exit):
+        """Sets the calculate_on_exit of this FormFieldCheckbox.
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :param own_status: The own_status of this FormFieldCheckbox.  # noqa: E501
+        :param calculate_on_exit: The calculate_on_exit of this FormFieldCheckbox.  # noqa: E501
         :type: bool
         """
-        self._own_status = own_status
+        self._calculate_on_exit = calculate_on_exit
 
     @property
-    def status_text(self):
-        """Gets the status_text of this FormFieldCheckbox.  # noqa: E501
+    def entry_macro(self):
+        """Gets the entry_macro of this FormFieldCheckbox.  # noqa: E501
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :return: The status_text of this FormFieldCheckbox.  # noqa: E501
+        :return: The entry_macro of this FormFieldCheckbox.  # noqa: E501
         :rtype: str
         """
-        return self._status_text
+        return self._entry_macro
 
-    @status_text.setter
-    def status_text(self, status_text):
-        """Sets the status_text of this FormFieldCheckbox.
+    @entry_macro.setter
+    def entry_macro(self, entry_macro):
+        """Sets the entry_macro of this FormFieldCheckbox.
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :param status_text: The status_text of this FormFieldCheckbox.  # noqa: E501
+        :param entry_macro: The entry_macro of this FormFieldCheckbox.  # noqa: E501
         :type: str
         """
-        self._status_text = status_text
+        self._entry_macro = entry_macro
+
+    @property
+    def exit_macro(self):
+        """Gets the exit_macro of this FormFieldCheckbox.  # noqa: E501
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :return: The exit_macro of this FormFieldCheckbox.  # noqa: E501
+        :rtype: str
+        """
+        return self._exit_macro
+
+    @exit_macro.setter
+    def exit_macro(self, exit_macro):
+        """Sets the exit_macro of this FormFieldCheckbox.
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :param exit_macro: The exit_macro of this FormFieldCheckbox.  # noqa: E501
+        :type: str
+        """
+        self._exit_macro = exit_macro
+
+    @property
+    def is_check_box_exact_size(self):
+        """Gets the is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
+
+        Gets or sets a value indicating whether the size of the textbox is automatic or specified explicitly.  # noqa: E501
+
+        :return: The is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
+        :rtype: bool
+        """
+        return self._is_check_box_exact_size
+
+    @is_check_box_exact_size.setter
+    def is_check_box_exact_size(self, is_check_box_exact_size):
+        """Sets the is_check_box_exact_size of this FormFieldCheckbox.
+
+        Gets or sets a value indicating whether the size of the textbox is automatic or specified explicitly.  # noqa: E501
+
+        :param is_check_box_exact_size: The is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
+        :type: bool
+        """
+        self._is_check_box_exact_size = is_check_box_exact_size
 
     @property
     def check_box_size(self):
         """Gets the check_box_size of this FormFieldCheckbox.  # noqa: E501
 
         Gets or sets the size of the checkbox in points. Has effect only when IsCheckBoxExactSize is true.  # noqa: E501
 
@@ -405,36 +427,14 @@
         Gets or sets the checked status of the check box form field.  # noqa: E501
 
         :param checked: The checked of this FormFieldCheckbox.  # noqa: E501
         :type: bool
         """
         self._checked = checked
 
-    @property
-    def is_check_box_exact_size(self):
-        """Gets the is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
-
-        Gets or sets a value indicating whether the size of the textbox is automatic or specified explicitly.  # noqa: E501
-
-        :return: The is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
-        :rtype: bool
-        """
-        return self._is_check_box_exact_size
-
-    @is_check_box_exact_size.setter
-    def is_check_box_exact_size(self, is_check_box_exact_size):
-        """Sets the is_check_box_exact_size of this FormFieldCheckbox.
-
-        Gets or sets a value indicating whether the size of the textbox is automatic or specified explicitly.  # noqa: E501
-
-        :param is_check_box_exact_size: The is_check_box_exact_size of this FormFieldCheckbox.  # noqa: E501
-        :type: bool
-        """
-        self._is_check_box_exact_size = is_check_box_exact_size
-
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section_link_collection_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/range_document.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/range_document.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/story_child_nodes.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/story_child_nodes.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/split_document_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/split_document_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/downsample_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/downsample_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_digital_signature_details_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_digital_signature_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_objects_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_objects_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,48 +39,48 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'allow_break_across_pages': 'bool',
-        'heading_format': 'bool',
         'height': 'float',
-        'height_rule': 'str'
+        'height_rule': 'str',
+        'allow_break_across_pages': 'bool',
+        'heading_format': 'bool'
     }
 
     attribute_map = {
         'link': 'Link',
-        'allow_break_across_pages': 'AllowBreakAcrossPages',
-        'heading_format': 'HeadingFormat',
         'height': 'Height',
-        'height_rule': 'HeightRule'
+        'height_rule': 'HeightRule',
+        'allow_break_across_pages': 'AllowBreakAcrossPages',
+        'heading_format': 'HeadingFormat'
     }
 
-    def __init__(self, link=None, allow_break_across_pages=None, heading_format=None, height=None, height_rule=None):  # noqa: E501
+    def __init__(self, link=None, height=None, height_rule=None, allow_break_across_pages=None, heading_format=None):  # noqa: E501
         """TableRowFormat - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._allow_break_across_pages = None
-        self._heading_format = None
         self._height = None
         self._height_rule = None
+        self._allow_break_across_pages = None
+        self._heading_format = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if allow_break_across_pages is not None:
-            self.allow_break_across_pages = allow_break_across_pages
-        if heading_format is not None:
-            self.heading_format = heading_format
         if height is not None:
             self.height = height
         if height_rule is not None:
             self.height_rule = height_rule
+        if allow_break_across_pages is not None:
+            self.allow_break_across_pages = allow_break_across_pages
+        if heading_format is not None:
+            self.heading_format = heading_format
 
     @property
     def link(self):
         """Gets the link of this TableRowFormat.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -97,58 +97,14 @@
 
         :param link: The link of this TableRowFormat.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def allow_break_across_pages(self):
-        """Gets the allow_break_across_pages of this TableRowFormat.  # noqa: E501
-
-        Gets or sets a value indicating whether the text in a table row is allowed to split across a page break.  # noqa: E501
-
-        :return: The allow_break_across_pages of this TableRowFormat.  # noqa: E501
-        :rtype: bool
-        """
-        return self._allow_break_across_pages
-
-    @allow_break_across_pages.setter
-    def allow_break_across_pages(self, allow_break_across_pages):
-        """Sets the allow_break_across_pages of this TableRowFormat.
-
-        Gets or sets a value indicating whether the text in a table row is allowed to split across a page break.  # noqa: E501
-
-        :param allow_break_across_pages: The allow_break_across_pages of this TableRowFormat.  # noqa: E501
-        :type: bool
-        """
-        self._allow_break_across_pages = allow_break_across_pages
-
-    @property
-    def heading_format(self):
-        """Gets the heading_format of this TableRowFormat.  # noqa: E501
-
-        Gets or sets a value indicating whether the row is repeated as a table heading on every page when the table spans more than one page.  # noqa: E501
-
-        :return: The heading_format of this TableRowFormat.  # noqa: E501
-        :rtype: bool
-        """
-        return self._heading_format
-
-    @heading_format.setter
-    def heading_format(self, heading_format):
-        """Sets the heading_format of this TableRowFormat.
-
-        Gets or sets a value indicating whether the row is repeated as a table heading on every page when the table spans more than one page.  # noqa: E501
-
-        :param heading_format: The heading_format of this TableRowFormat.  # noqa: E501
-        :type: bool
-        """
-        self._heading_format = heading_format
-
-    @property
     def height(self):
         """Gets the height of this TableRowFormat.  # noqa: E501
 
         Gets or sets the height of the table row in points.  # noqa: E501
 
         :return: The height of this TableRowFormat.  # noqa: E501
         :rtype: float
@@ -192,14 +148,58 @@
                 raise ValueError(
                     "Invalid value for `height_rule` ({0}), must be one of {1}"  # noqa: E501
                     .format(height_rule, allowed_values))
             self._height_rule = height_rule
         else:
             self._height_rule = allowed_values[int(height_rule) if six.PY3 else long(height_rule)]
 
+    @property
+    def allow_break_across_pages(self):
+        """Gets the allow_break_across_pages of this TableRowFormat.  # noqa: E501
+
+        Gets or sets a value indicating whether the text in a table row is allowed to split across a page break.  # noqa: E501
+
+        :return: The allow_break_across_pages of this TableRowFormat.  # noqa: E501
+        :rtype: bool
+        """
+        return self._allow_break_across_pages
+
+    @allow_break_across_pages.setter
+    def allow_break_across_pages(self, allow_break_across_pages):
+        """Sets the allow_break_across_pages of this TableRowFormat.
+
+        Gets or sets a value indicating whether the text in a table row is allowed to split across a page break.  # noqa: E501
+
+        :param allow_break_across_pages: The allow_break_across_pages of this TableRowFormat.  # noqa: E501
+        :type: bool
+        """
+        self._allow_break_across_pages = allow_break_across_pages
+
+    @property
+    def heading_format(self):
+        """Gets the heading_format of this TableRowFormat.  # noqa: E501
+
+        Gets or sets a value indicating whether the row is repeated as a table heading on every page when the table spans more than one page.  # noqa: E501
+
+        :return: The heading_format of this TableRowFormat.  # noqa: E501
+        :rtype: bool
+        """
+        return self._heading_format
+
+    @heading_format.setter
+    def heading_format(self, heading_format):
+        """Sets the heading_format of this TableRowFormat.
+
+        Gets or sets a value indicating whether the row is repeated as a table heading on every page when the table spans more than one page.  # noqa: E501
+
+        :param heading_format: The heading_format of this TableRowFormat.  # noqa: E501
+        :type: bool
+        """
+        self._heading_format = heading_format
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/save_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/save_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,61 +38,39 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'additional_items': 'list[FileLink]',
         'dest_document': 'FileLink',
-        'source_document': 'FileLink'
+        'source_document': 'FileLink',
+        'additional_items': 'list[FileLink]'
     }
 
     attribute_map = {
-        'additional_items': 'AdditionalItems',
         'dest_document': 'DestDocument',
-        'source_document': 'SourceDocument'
+        'source_document': 'SourceDocument',
+        'additional_items': 'AdditionalItems'
     }
 
-    def __init__(self, additional_items=None, dest_document=None, source_document=None):  # noqa: E501
+    def __init__(self, dest_document=None, source_document=None, additional_items=None):  # noqa: E501
         """SaveResult - a model defined in Swagger"""  # noqa: E501
 
-        self._additional_items = None
         self._dest_document = None
         self._source_document = None
+        self._additional_items = None
         self.discriminator = None
 
-        if additional_items is not None:
-            self.additional_items = additional_items
         if dest_document is not None:
             self.dest_document = dest_document
         if source_document is not None:
             self.source_document = source_document
-
-    @property
-    def additional_items(self):
-        """Gets the additional_items of this SaveResult.  # noqa: E501
-
-        Gets or sets the list of links to additional items (css, images etc).  # noqa: E501
-
-        :return: The additional_items of this SaveResult.  # noqa: E501
-        :rtype: list[FileLink]
-        """
-        return self._additional_items
-
-    @additional_items.setter
-    def additional_items(self, additional_items):
-        """Sets the additional_items of this SaveResult.
-
-        Gets or sets the list of links to additional items (css, images etc).  # noqa: E501
-
-        :param additional_items: The additional_items of this SaveResult.  # noqa: E501
-        :type: list[FileLink]
-        """
-        self._additional_items = additional_items
+        if additional_items is not None:
+            self.additional_items = additional_items
 
     @property
     def dest_document(self):
         """Gets the dest_document of this SaveResult.  # noqa: E501
 
         Gets or sets the link to destination document.  # noqa: E501
 
@@ -130,14 +108,36 @@
         Gets or sets the link to source document.  # noqa: E501
 
         :param source_document: The source_document of this SaveResult.  # noqa: E501
         :type: FileLink
         """
         self._source_document = source_document
 
+    @property
+    def additional_items(self):
+        """Gets the additional_items of this SaveResult.  # noqa: E501
+
+        Gets or sets the list of links to additional items (css, images etc).  # noqa: E501
+
+        :return: The additional_items of this SaveResult.  # noqa: E501
+        :rtype: list[FileLink]
+        """
+        return self._additional_items
+
+    @additional_items.setter
+    def additional_items(self, additional_items):
+        """Sets the additional_items of this SaveResult.
+
+        Gets or sets the list of links to additional items (css, images etc).  # noqa: E501
+
+        :param additional_items: The additional_items of this SaveResult.  # noqa: E501
+        :type: list[FileLink]
+        """
+        self._additional_items = additional_items
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/open_xps_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/open_xps_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/optimization_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/optimization_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/replace_range_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_object.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/styles_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/styles_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/protection_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_macro_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/image_entry.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/image_entry.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comment.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comment.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,63 +39,63 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
+        'range_start': 'DocumentPosition',
+        'range_end': 'DocumentPosition',
         'author': 'str',
-        'content': 'StoryChildNodes',
-        'date_time': 'datetime',
         'initial': 'str',
-        'range_end': 'DocumentPosition',
-        'range_start': 'DocumentPosition',
-        'text': 'str'
+        'date_time': 'datetime',
+        'text': 'str',
+        'content': 'StoryChildNodes'
     }
 
     attribute_map = {
         'link': 'Link',
+        'range_start': 'RangeStart',
+        'range_end': 'RangeEnd',
         'author': 'Author',
-        'content': 'Content',
-        'date_time': 'DateTime',
         'initial': 'Initial',
-        'range_end': 'RangeEnd',
-        'range_start': 'RangeStart',
-        'text': 'Text'
+        'date_time': 'DateTime',
+        'text': 'Text',
+        'content': 'Content'
     }
 
-    def __init__(self, link=None, author=None, content=None, date_time=None, initial=None, range_end=None, range_start=None, text=None):  # noqa: E501
+    def __init__(self, link=None, range_start=None, range_end=None, author=None, initial=None, date_time=None, text=None, content=None):  # noqa: E501
         """Comment - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
+        self._range_start = None
+        self._range_end = None
         self._author = None
-        self._content = None
-        self._date_time = None
         self._initial = None
-        self._range_end = None
-        self._range_start = None
+        self._date_time = None
         self._text = None
+        self._content = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
+        if range_start is not None:
+            self.range_start = range_start
+        if range_end is not None:
+            self.range_end = range_end
         if author is not None:
             self.author = author
-        if content is not None:
-            self.content = content
-        if date_time is not None:
-            self.date_time = date_time
         if initial is not None:
             self.initial = initial
-        if range_end is not None:
-            self.range_end = range_end
-        if range_start is not None:
-            self.range_start = range_start
+        if date_time is not None:
+            self.date_time = date_time
         if text is not None:
             self.text = text
+        if content is not None:
+            self.content = content
 
     @property
     def link(self):
         """Gets the link of this Comment.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -112,78 +112,78 @@
 
         :param link: The link of this Comment.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def author(self):
-        """Gets the author of this Comment.  # noqa: E501
+    def range_start(self):
+        """Gets the range_start of this Comment.  # noqa: E501
 
-        Gets or sets the author name for a comment.  # noqa: E501
+        Gets or sets the link to comment range start node.  # noqa: E501
 
-        :return: The author of this Comment.  # noqa: E501
-        :rtype: str
+        :return: The range_start of this Comment.  # noqa: E501
+        :rtype: DocumentPosition
         """
-        return self._author
+        return self._range_start
 
-    @author.setter
-    def author(self, author):
-        """Sets the author of this Comment.
+    @range_start.setter
+    def range_start(self, range_start):
+        """Sets the range_start of this Comment.
 
-        Gets or sets the author name for a comment.  # noqa: E501
+        Gets or sets the link to comment range start node.  # noqa: E501
 
-        :param author: The author of this Comment.  # noqa: E501
-        :type: str
+        :param range_start: The range_start of this Comment.  # noqa: E501
+        :type: DocumentPosition
         """
-        self._author = author
+        self._range_start = range_start
 
     @property
-    def content(self):
-        """Gets the content of this Comment.  # noqa: E501
+    def range_end(self):
+        """Gets the range_end of this Comment.  # noqa: E501
 
-        Gets or sets the content of the comment.  # noqa: E501
+        Gets or sets the link to comment range end node.  # noqa: E501
 
-        :return: The content of this Comment.  # noqa: E501
-        :rtype: StoryChildNodes
+        :return: The range_end of this Comment.  # noqa: E501
+        :rtype: DocumentPosition
         """
-        return self._content
+        return self._range_end
 
-    @content.setter
-    def content(self, content):
-        """Sets the content of this Comment.
+    @range_end.setter
+    def range_end(self, range_end):
+        """Sets the range_end of this Comment.
 
-        Gets or sets the content of the comment.  # noqa: E501
+        Gets or sets the link to comment range end node.  # noqa: E501
 
-        :param content: The content of this Comment.  # noqa: E501
-        :type: StoryChildNodes
+        :param range_end: The range_end of this Comment.  # noqa: E501
+        :type: DocumentPosition
         """
-        self._content = content
+        self._range_end = range_end
 
     @property
-    def date_time(self):
-        """Gets the date_time of this Comment.  # noqa: E501
+    def author(self):
+        """Gets the author of this Comment.  # noqa: E501
 
-        Gets or sets the date and time that the comment was made.  # noqa: E501
+        Gets or sets the author name for a comment.  # noqa: E501
 
-        :return: The date_time of this Comment.  # noqa: E501
-        :rtype: datetime
+        :return: The author of this Comment.  # noqa: E501
+        :rtype: str
         """
-        return self._date_time
+        return self._author
 
-    @date_time.setter
-    def date_time(self, date_time):
-        """Sets the date_time of this Comment.
+    @author.setter
+    def author(self, author):
+        """Sets the author of this Comment.
 
-        Gets or sets the date and time that the comment was made.  # noqa: E501
+        Gets or sets the author name for a comment.  # noqa: E501
 
-        :param date_time: The date_time of this Comment.  # noqa: E501
-        :type: datetime
+        :param author: The author of this Comment.  # noqa: E501
+        :type: str
         """
-        self._date_time = date_time
+        self._author = author
 
     @property
     def initial(self):
         """Gets the initial of this Comment.  # noqa: E501
 
         Gets or sets the initials of the user associated with a specific comment.  # noqa: E501
 
@@ -200,56 +200,34 @@
 
         :param initial: The initial of this Comment.  # noqa: E501
         :type: str
         """
         self._initial = initial
 
     @property
-    def range_end(self):
-        """Gets the range_end of this Comment.  # noqa: E501
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :return: The range_end of this Comment.  # noqa: E501
-        :rtype: DocumentPosition
-        """
-        return self._range_end
-
-    @range_end.setter
-    def range_end(self, range_end):
-        """Sets the range_end of this Comment.
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :param range_end: The range_end of this Comment.  # noqa: E501
-        :type: DocumentPosition
-        """
-        self._range_end = range_end
-
-    @property
-    def range_start(self):
-        """Gets the range_start of this Comment.  # noqa: E501
+    def date_time(self):
+        """Gets the date_time of this Comment.  # noqa: E501
 
-        Gets or sets the link to comment range start node.  # noqa: E501
+        Gets or sets the date and time that the comment was made.  # noqa: E501
 
-        :return: The range_start of this Comment.  # noqa: E501
-        :rtype: DocumentPosition
+        :return: The date_time of this Comment.  # noqa: E501
+        :rtype: datetime
         """
-        return self._range_start
+        return self._date_time
 
-    @range_start.setter
-    def range_start(self, range_start):
-        """Sets the range_start of this Comment.
+    @date_time.setter
+    def date_time(self, date_time):
+        """Sets the date_time of this Comment.
 
-        Gets or sets the link to comment range start node.  # noqa: E501
+        Gets or sets the date and time that the comment was made.  # noqa: E501
 
-        :param range_start: The range_start of this Comment.  # noqa: E501
-        :type: DocumentPosition
+        :param date_time: The date_time of this Comment.  # noqa: E501
+        :type: datetime
         """
-        self._range_start = range_start
+        self._date_time = date_time
 
     @property
     def text(self):
         """Gets the text of this Comment.  # noqa: E501
 
         Gets or sets text of the comment.  # noqa: E501
 
@@ -265,14 +243,36 @@
         Gets or sets text of the comment.  # noqa: E501
 
         :param text: The text of this Comment.  # noqa: E501
         :type: str
         """
         self._text = text
 
+    @property
+    def content(self):
+        """Gets the content of this Comment.  # noqa: E501
+
+        Gets or sets the content of the comment.  # noqa: E501
+
+        :return: The content of this Comment.  # noqa: E501
+        :rtype: StoryChildNodes
+        """
+        return self._content
+
+    @content.setter
+    def content(self, content):
+        """Sets the content of this Comment.
+
+        Gets or sets the content of the comment.  # noqa: E501
+
+        :param content: The content of this Comment.  # noqa: E501
+        :type: StoryChildNodes
+        """
+        self._content = content
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/compress_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/compress_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/odt_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/odt_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_drop_down.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_drop_down.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,83 +40,83 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'calculate_on_exit': 'bool',
+        'name': 'str',
         'enabled': 'bool',
-        'entry_macro': 'str',
-        'exit_macro': 'str',
+        'status_text': 'str',
+        'own_status': 'bool',
         'help_text': 'str',
-        'name': 'str',
         'own_help': 'bool',
-        'own_status': 'bool',
-        'status_text': 'str',
+        'calculate_on_exit': 'bool',
+        'entry_macro': 'str',
+        'exit_macro': 'str',
         'drop_down_items': 'list[str]',
         'drop_down_selected_index': 'int'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'calculate_on_exit': 'CalculateOnExit',
+        'name': 'Name',
         'enabled': 'Enabled',
-        'entry_macro': 'EntryMacro',
-        'exit_macro': 'ExitMacro',
+        'status_text': 'StatusText',
+        'own_status': 'OwnStatus',
         'help_text': 'HelpText',
-        'name': 'Name',
         'own_help': 'OwnHelp',
-        'own_status': 'OwnStatus',
-        'status_text': 'StatusText',
+        'calculate_on_exit': 'CalculateOnExit',
+        'entry_macro': 'EntryMacro',
+        'exit_macro': 'ExitMacro',
         'drop_down_items': 'DropDownItems',
         'drop_down_selected_index': 'DropDownSelectedIndex'
     }
 
-    def __init__(self, link=None, node_id=None, calculate_on_exit=None, enabled=None, entry_macro=None, exit_macro=None, help_text=None, name=None, own_help=None, own_status=None, status_text=None, drop_down_items=None, drop_down_selected_index=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, name=None, enabled=None, status_text=None, own_status=None, help_text=None, own_help=None, calculate_on_exit=None, entry_macro=None, exit_macro=None, drop_down_items=None, drop_down_selected_index=None):  # noqa: E501
         """FormFieldDropDown - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._calculate_on_exit = None
+        self._name = None
         self._enabled = None
-        self._entry_macro = None
-        self._exit_macro = None
+        self._status_text = None
+        self._own_status = None
         self._help_text = None
-        self._name = None
         self._own_help = None
-        self._own_status = None
-        self._status_text = None
+        self._calculate_on_exit = None
+        self._entry_macro = None
+        self._exit_macro = None
         self._drop_down_items = None
         self._drop_down_selected_index = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if calculate_on_exit is not None:
-            self.calculate_on_exit = calculate_on_exit
+        if name is not None:
+            self.name = name
         if enabled is not None:
             self.enabled = enabled
-        if entry_macro is not None:
-            self.entry_macro = entry_macro
-        if exit_macro is not None:
-            self.exit_macro = exit_macro
+        if status_text is not None:
+            self.status_text = status_text
+        if own_status is not None:
+            self.own_status = own_status
         if help_text is not None:
             self.help_text = help_text
-        if name is not None:
-            self.name = name
         if own_help is not None:
             self.own_help = own_help
-        if own_status is not None:
-            self.own_status = own_status
-        if status_text is not None:
-            self.status_text = status_text
+        if calculate_on_exit is not None:
+            self.calculate_on_exit = calculate_on_exit
+        if entry_macro is not None:
+            self.entry_macro = entry_macro
+        if exit_macro is not None:
+            self.exit_macro = exit_macro
         if drop_down_items is not None:
             self.drop_down_items = drop_down_items
         if drop_down_selected_index is not None:
             self.drop_down_selected_index = drop_down_selected_index
 
     @property
     def link(self):
@@ -159,34 +159,34 @@
 
         :param node_id: The node_id of this FormFieldDropDown.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def calculate_on_exit(self):
-        """Gets the calculate_on_exit of this FormFieldDropDown.  # noqa: E501
+    def name(self):
+        """Gets the name of this FormFieldDropDown.  # noqa: E501
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :return: The calculate_on_exit of this FormFieldDropDown.  # noqa: E501
-        :rtype: bool
+        :return: The name of this FormFieldDropDown.  # noqa: E501
+        :rtype: str
         """
-        return self._calculate_on_exit
+        return self._name
 
-    @calculate_on_exit.setter
-    def calculate_on_exit(self, calculate_on_exit):
-        """Sets the calculate_on_exit of this FormFieldDropDown.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this FormFieldDropDown.
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :param calculate_on_exit: The calculate_on_exit of this FormFieldDropDown.  # noqa: E501
-        :type: bool
+        :param name: The name of this FormFieldDropDown.  # noqa: E501
+        :type: str
         """
-        self._calculate_on_exit = calculate_on_exit
+        self._name = name
 
     @property
     def enabled(self):
         """Gets the enabled of this FormFieldDropDown.  # noqa: E501
 
         Gets or sets a value indicating whether a form field is enabled.  # noqa: E501
 
@@ -203,56 +203,56 @@
 
         :param enabled: The enabled of this FormFieldDropDown.  # noqa: E501
         :type: bool
         """
         self._enabled = enabled
 
     @property
-    def entry_macro(self):
-        """Gets the entry_macro of this FormFieldDropDown.  # noqa: E501
+    def status_text(self):
+        """Gets the status_text of this FormFieldDropDown.  # noqa: E501
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The entry_macro of this FormFieldDropDown.  # noqa: E501
+        :return: The status_text of this FormFieldDropDown.  # noqa: E501
         :rtype: str
         """
-        return self._entry_macro
+        return self._status_text
 
-    @entry_macro.setter
-    def entry_macro(self, entry_macro):
-        """Sets the entry_macro of this FormFieldDropDown.
+    @status_text.setter
+    def status_text(self, status_text):
+        """Sets the status_text of this FormFieldDropDown.
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param entry_macro: The entry_macro of this FormFieldDropDown.  # noqa: E501
+        :param status_text: The status_text of this FormFieldDropDown.  # noqa: E501
         :type: str
         """
-        self._entry_macro = entry_macro
+        self._status_text = status_text
 
     @property
-    def exit_macro(self):
-        """Gets the exit_macro of this FormFieldDropDown.  # noqa: E501
+    def own_status(self):
+        """Gets the own_status of this FormFieldDropDown.  # noqa: E501
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The exit_macro of this FormFieldDropDown.  # noqa: E501
-        :rtype: str
+        :return: The own_status of this FormFieldDropDown.  # noqa: E501
+        :rtype: bool
         """
-        return self._exit_macro
+        return self._own_status
 
-    @exit_macro.setter
-    def exit_macro(self, exit_macro):
-        """Sets the exit_macro of this FormFieldDropDown.
+    @own_status.setter
+    def own_status(self, own_status):
+        """Sets the own_status of this FormFieldDropDown.
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param exit_macro: The exit_macro of this FormFieldDropDown.  # noqa: E501
-        :type: str
+        :param own_status: The own_status of this FormFieldDropDown.  # noqa: E501
+        :type: bool
         """
-        self._exit_macro = exit_macro
+        self._own_status = own_status
 
     @property
     def help_text(self):
         """Gets the help_text of this FormFieldDropDown.  # noqa: E501
 
         Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1.  # noqa: E501
 
@@ -269,36 +269,14 @@
 
         :param help_text: The help_text of this FormFieldDropDown.  # noqa: E501
         :type: str
         """
         self._help_text = help_text
 
     @property
-    def name(self):
-        """Gets the name of this FormFieldDropDown.  # noqa: E501
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :return: The name of this FormFieldDropDown.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this FormFieldDropDown.
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :param name: The name of this FormFieldDropDown.  # noqa: E501
-        :type: str
-        """
-        self._name = name
-
-    @property
     def own_help(self):
         """Gets the own_help of this FormFieldDropDown.  # noqa: E501
 
         Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1.  # noqa: E501
 
         :return: The own_help of this FormFieldDropDown.  # noqa: E501
         :rtype: bool
@@ -313,56 +291,78 @@
 
         :param own_help: The own_help of this FormFieldDropDown.  # noqa: E501
         :type: bool
         """
         self._own_help = own_help
 
     @property
-    def own_status(self):
-        """Gets the own_status of this FormFieldDropDown.  # noqa: E501
+    def calculate_on_exit(self):
+        """Gets the calculate_on_exit of this FormFieldDropDown.  # noqa: E501
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :return: The own_status of this FormFieldDropDown.  # noqa: E501
+        :return: The calculate_on_exit of this FormFieldDropDown.  # noqa: E501
         :rtype: bool
         """
-        return self._own_status
+        return self._calculate_on_exit
 
-    @own_status.setter
-    def own_status(self, own_status):
-        """Sets the own_status of this FormFieldDropDown.
+    @calculate_on_exit.setter
+    def calculate_on_exit(self, calculate_on_exit):
+        """Sets the calculate_on_exit of this FormFieldDropDown.
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :param own_status: The own_status of this FormFieldDropDown.  # noqa: E501
+        :param calculate_on_exit: The calculate_on_exit of this FormFieldDropDown.  # noqa: E501
         :type: bool
         """
-        self._own_status = own_status
+        self._calculate_on_exit = calculate_on_exit
 
     @property
-    def status_text(self):
-        """Gets the status_text of this FormFieldDropDown.  # noqa: E501
+    def entry_macro(self):
+        """Gets the entry_macro of this FormFieldDropDown.  # noqa: E501
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :return: The status_text of this FormFieldDropDown.  # noqa: E501
+        :return: The entry_macro of this FormFieldDropDown.  # noqa: E501
         :rtype: str
         """
-        return self._status_text
+        return self._entry_macro
 
-    @status_text.setter
-    def status_text(self, status_text):
-        """Sets the status_text of this FormFieldDropDown.
+    @entry_macro.setter
+    def entry_macro(self, entry_macro):
+        """Sets the entry_macro of this FormFieldDropDown.
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :param status_text: The status_text of this FormFieldDropDown.  # noqa: E501
+        :param entry_macro: The entry_macro of this FormFieldDropDown.  # noqa: E501
         :type: str
         """
-        self._status_text = status_text
+        self._entry_macro = entry_macro
+
+    @property
+    def exit_macro(self):
+        """Gets the exit_macro of this FormFieldDropDown.  # noqa: E501
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :return: The exit_macro of this FormFieldDropDown.  # noqa: E501
+        :rtype: str
+        """
+        return self._exit_macro
+
+    @exit_macro.setter
+    def exit_macro(self, exit_macro):
+        """Sets the exit_macro of this FormFieldDropDown.
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :param exit_macro: The exit_macro of this FormFieldDropDown.  # noqa: E501
+        :type: str
+        """
+        self._exit_macro = exit_macro
 
     @property
     def drop_down_items(self):
         """Gets the drop_down_items of this FormFieldDropDown.  # noqa: E501
 
         Gets or sets the items array of a dropdown form field.  # noqa: E501
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_info.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,63 +39,63 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'is_list_style_definition': 'bool',
-        'is_list_style_reference': 'bool',
+        'list_id': 'int',
         'is_multi_level': 'bool',
         'is_restart_at_each_section': 'bool',
-        'list_id': 'int',
-        'list_levels': 'ListLevels',
-        'style': 'Style'
+        'is_list_style_definition': 'bool',
+        'is_list_style_reference': 'bool',
+        'style': 'Style',
+        'list_levels': 'ListLevels'
     }
 
     attribute_map = {
         'link': 'Link',
-        'is_list_style_definition': 'IsListStyleDefinition',
-        'is_list_style_reference': 'IsListStyleReference',
+        'list_id': 'ListId',
         'is_multi_level': 'IsMultiLevel',
         'is_restart_at_each_section': 'IsRestartAtEachSection',
-        'list_id': 'ListId',
-        'list_levels': 'ListLevels',
-        'style': 'Style'
+        'is_list_style_definition': 'IsListStyleDefinition',
+        'is_list_style_reference': 'IsListStyleReference',
+        'style': 'Style',
+        'list_levels': 'ListLevels'
     }
 
-    def __init__(self, link=None, is_list_style_definition=None, is_list_style_reference=None, is_multi_level=None, is_restart_at_each_section=None, list_id=None, list_levels=None, style=None):  # noqa: E501
+    def __init__(self, link=None, list_id=None, is_multi_level=None, is_restart_at_each_section=None, is_list_style_definition=None, is_list_style_reference=None, style=None, list_levels=None):  # noqa: E501
         """ListInfo - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._is_list_style_definition = None
-        self._is_list_style_reference = None
+        self._list_id = None
         self._is_multi_level = None
         self._is_restart_at_each_section = None
-        self._list_id = None
-        self._list_levels = None
+        self._is_list_style_definition = None
+        self._is_list_style_reference = None
         self._style = None
+        self._list_levels = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if is_list_style_definition is not None:
-            self.is_list_style_definition = is_list_style_definition
-        if is_list_style_reference is not None:
-            self.is_list_style_reference = is_list_style_reference
+        if list_id is not None:
+            self.list_id = list_id
         if is_multi_level is not None:
             self.is_multi_level = is_multi_level
         if is_restart_at_each_section is not None:
             self.is_restart_at_each_section = is_restart_at_each_section
-        if list_id is not None:
-            self.list_id = list_id
-        if list_levels is not None:
-            self.list_levels = list_levels
+        if is_list_style_definition is not None:
+            self.is_list_style_definition = is_list_style_definition
+        if is_list_style_reference is not None:
+            self.is_list_style_reference = is_list_style_reference
         if style is not None:
             self.style = style
+        if list_levels is not None:
+            self.list_levels = list_levels
 
     @property
     def link(self):
         """Gets the link of this ListInfo.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -112,56 +112,34 @@
 
         :param link: The link of this ListInfo.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def is_list_style_definition(self):
-        """Gets the is_list_style_definition of this ListInfo.  # noqa: E501
-
-        Gets or sets a value indicating whether this list is a definition of a list style.  # noqa: E501
-
-        :return: The is_list_style_definition of this ListInfo.  # noqa: E501
-        :rtype: bool
-        """
-        return self._is_list_style_definition
-
-    @is_list_style_definition.setter
-    def is_list_style_definition(self, is_list_style_definition):
-        """Sets the is_list_style_definition of this ListInfo.
-
-        Gets or sets a value indicating whether this list is a definition of a list style.  # noqa: E501
-
-        :param is_list_style_definition: The is_list_style_definition of this ListInfo.  # noqa: E501
-        :type: bool
-        """
-        self._is_list_style_definition = is_list_style_definition
-
-    @property
-    def is_list_style_reference(self):
-        """Gets the is_list_style_reference of this ListInfo.  # noqa: E501
+    def list_id(self):
+        """Gets the list_id of this ListInfo.  # noqa: E501
 
-        Gets or sets a value indicating whether this list is a reference to a list style.  # noqa: E501
+        Gets or sets the unique identifier of the list.  # noqa: E501
 
-        :return: The is_list_style_reference of this ListInfo.  # noqa: E501
-        :rtype: bool
+        :return: The list_id of this ListInfo.  # noqa: E501
+        :rtype: int
         """
-        return self._is_list_style_reference
+        return self._list_id
 
-    @is_list_style_reference.setter
-    def is_list_style_reference(self, is_list_style_reference):
-        """Sets the is_list_style_reference of this ListInfo.
+    @list_id.setter
+    def list_id(self, list_id):
+        """Sets the list_id of this ListInfo.
 
-        Gets or sets a value indicating whether this list is a reference to a list style.  # noqa: E501
+        Gets or sets the unique identifier of the list.  # noqa: E501
 
-        :param is_list_style_reference: The is_list_style_reference of this ListInfo.  # noqa: E501
-        :type: bool
+        :param list_id: The list_id of this ListInfo.  # noqa: E501
+        :type: int
         """
-        self._is_list_style_reference = is_list_style_reference
+        self._list_id = list_id
 
     @property
     def is_multi_level(self):
         """Gets the is_multi_level of this ListInfo.  # noqa: E501
 
         Gets or sets a value indicating whether the list contains 9 levels; false when 1 level.  # noqa: E501
 
@@ -200,56 +178,56 @@
 
         :param is_restart_at_each_section: The is_restart_at_each_section of this ListInfo.  # noqa: E501
         :type: bool
         """
         self._is_restart_at_each_section = is_restart_at_each_section
 
     @property
-    def list_id(self):
-        """Gets the list_id of this ListInfo.  # noqa: E501
+    def is_list_style_definition(self):
+        """Gets the is_list_style_definition of this ListInfo.  # noqa: E501
 
-        Gets or sets the unique identifier of the list.  # noqa: E501
+        Gets or sets a value indicating whether this list is a definition of a list style.  # noqa: E501
 
-        :return: The list_id of this ListInfo.  # noqa: E501
-        :rtype: int
+        :return: The is_list_style_definition of this ListInfo.  # noqa: E501
+        :rtype: bool
         """
-        return self._list_id
+        return self._is_list_style_definition
 
-    @list_id.setter
-    def list_id(self, list_id):
-        """Sets the list_id of this ListInfo.
+    @is_list_style_definition.setter
+    def is_list_style_definition(self, is_list_style_definition):
+        """Sets the is_list_style_definition of this ListInfo.
 
-        Gets or sets the unique identifier of the list.  # noqa: E501
+        Gets or sets a value indicating whether this list is a definition of a list style.  # noqa: E501
 
-        :param list_id: The list_id of this ListInfo.  # noqa: E501
-        :type: int
+        :param is_list_style_definition: The is_list_style_definition of this ListInfo.  # noqa: E501
+        :type: bool
         """
-        self._list_id = list_id
+        self._is_list_style_definition = is_list_style_definition
 
     @property
-    def list_levels(self):
-        """Gets the list_levels of this ListInfo.  # noqa: E501
+    def is_list_style_reference(self):
+        """Gets the is_list_style_reference of this ListInfo.  # noqa: E501
 
-        Gets or sets the collection of list levels for this list.  # noqa: E501
+        Gets or sets a value indicating whether this list is a reference to a list style.  # noqa: E501
 
-        :return: The list_levels of this ListInfo.  # noqa: E501
-        :rtype: ListLevels
+        :return: The is_list_style_reference of this ListInfo.  # noqa: E501
+        :rtype: bool
         """
-        return self._list_levels
+        return self._is_list_style_reference
 
-    @list_levels.setter
-    def list_levels(self, list_levels):
-        """Sets the list_levels of this ListInfo.
+    @is_list_style_reference.setter
+    def is_list_style_reference(self, is_list_style_reference):
+        """Sets the is_list_style_reference of this ListInfo.
 
-        Gets or sets the collection of list levels for this list.  # noqa: E501
+        Gets or sets a value indicating whether this list is a reference to a list style.  # noqa: E501
 
-        :param list_levels: The list_levels of this ListInfo.  # noqa: E501
-        :type: ListLevels
+        :param is_list_style_reference: The is_list_style_reference of this ListInfo.  # noqa: E501
+        :type: bool
         """
-        self._list_levels = list_levels
+        self._is_list_style_reference = is_list_style_reference
 
     @property
     def style(self):
         """Gets the style of this ListInfo.  # noqa: E501
 
         Gets or sets the list style that this list references or defines.  # noqa: E501
 
@@ -265,14 +243,36 @@
         Gets or sets the list style that this list references or defines.  # noqa: E501
 
         :param style: The style of this ListInfo.  # noqa: E501
         :type: Style
         """
         self._style = style
 
+    @property
+    def list_levels(self):
+        """Gets the list_levels of this ListInfo.  # noqa: E501
+
+        Gets or sets the collection of list levels for this list.  # noqa: E501
+
+        :return: The list_levels of this ListInfo.  # noqa: E501
+        :rtype: ListLevels
+        """
+        return self._list_levels
+
+    @list_levels.setter
+    def list_levels(self, list_levels):
+        """Sets the list_levels of this ListInfo.
+
+        Gets or sets the collection of list levels for this list.  # noqa: E501
+
+        :param list_levels: The list_levels of this ListInfo.  # noqa: E501
+        :type: ListLevels
+        """
+        self._list_levels = list_levels
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/classification_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/classification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_format_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/compare_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/compare_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/rtf_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/rtf_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         'update_last_printed_property': 'bool',
         'update_last_saved_time_property': 'bool',
         'update_sdt_content': 'bool',
         'zip_output': 'bool',
         'export_compact_size': 'bool',
         'export_images_for_old_readers': 'bool',
         'pretty_format': 'bool',
-        'save_format': 'str',
-        'save_images_as_wmf': 'bool'
+        'save_images_as_wmf': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -75,16 +75,16 @@
         'update_last_printed_property': 'UpdateLastPrintedProperty',
         'update_last_saved_time_property': 'UpdateLastSavedTimeProperty',
         'update_sdt_content': 'UpdateSdtContent',
         'zip_output': 'ZipOutput',
         'export_compact_size': 'ExportCompactSize',
         'export_images_for_old_readers': 'ExportImagesForOldReaders',
         'pretty_format': 'PrettyFormat',
-        'save_format': 'SaveFormat',
-        'save_images_as_wmf': 'SaveImagesAsWmf'
+        'save_images_as_wmf': 'SaveImagesAsWmf',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, export_compact_size=None, export_images_for_old_readers=None, pretty_format=None, save_images_as_wmf=None):  # noqa: E501
         """RtfSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -98,16 +98,16 @@
         self._update_last_printed_property = None
         self._update_last_saved_time_property = None
         self._update_sdt_content = None
         self._zip_output = None
         self._export_compact_size = None
         self._export_images_for_old_readers = None
         self._pretty_format = None
-        self._save_format = "rtf"
         self._save_images_as_wmf = None
+        self._save_format = "rtf"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -522,26 +522,14 @@
 
         :param pretty_format: The pretty_format of this RtfSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._pretty_format = pretty_format
 
     @property
-    def save_format(self):
-        """Gets the save_format of this RtfSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this RtfSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def save_images_as_wmf(self):
         """Gets the save_images_as_wmf of this RtfSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether when true all images will be saved as WMF. This option might help to avoid WordPad warning messages.  # noqa: E501
 
         :return: The save_images_as_wmf of this RtfSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -555,14 +543,26 @@
         Gets or sets a value indicating whether when true all images will be saved as WMF. This option might help to avoid WordPad warning messages.  # noqa: E501
 
         :param save_images_as_wmf: The save_images_as_wmf of this RtfSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._save_images_as_wmf = save_images_as_wmf
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this RtfSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this RtfSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/watermark_text.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/watermark_text.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_property.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,43 +39,43 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'built_in': 'bool',
         'name': 'str',
-        'value': 'str'
+        'value': 'str',
+        'built_in': 'bool'
     }
 
     attribute_map = {
         'link': 'Link',
-        'built_in': 'BuiltIn',
         'name': 'Name',
-        'value': 'Value'
+        'value': 'Value',
+        'built_in': 'BuiltIn'
     }
 
-    def __init__(self, link=None, built_in=None, name=None, value=None):  # noqa: E501
+    def __init__(self, link=None, name=None, value=None, built_in=None):  # noqa: E501
         """DocumentProperty - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._built_in = None
         self._name = None
         self._value = None
+        self._built_in = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if built_in is not None:
-            self.built_in = built_in
         if name is not None:
             self.name = name
         if value is not None:
             self.value = value
+        if built_in is not None:
+            self.built_in = built_in
 
     @property
     def link(self):
         """Gets the link of this DocumentProperty.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -92,36 +92,14 @@
 
         :param link: The link of this DocumentProperty.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def built_in(self):
-        """Gets the built_in of this DocumentProperty.  # noqa: E501
-
-        Gets or sets a value indicating whether the property is built-in or not. If true the property is built-in, if false the property is custom.  # noqa: E501
-
-        :return: The built_in of this DocumentProperty.  # noqa: E501
-        :rtype: bool
-        """
-        return self._built_in
-
-    @built_in.setter
-    def built_in(self, built_in):
-        """Sets the built_in of this DocumentProperty.
-
-        Gets or sets a value indicating whether the property is built-in or not. If true the property is built-in, if false the property is custom.  # noqa: E501
-
-        :param built_in: The built_in of this DocumentProperty.  # noqa: E501
-        :type: bool
-        """
-        self._built_in = built_in
-
-    @property
     def name(self):
         """Gets the name of this DocumentProperty.  # noqa: E501
 
         Gets or sets the name of the document property.  # noqa: E501
 
         :return: The name of this DocumentProperty.  # noqa: E501
         :rtype: str
@@ -157,14 +135,36 @@
         Gets or sets the value of the document property.  # noqa: E501
 
         :param value: The value of this DocumentProperty.  # noqa: E501
         :type: str
         """
         self._value = value
 
+    @property
+    def built_in(self):
+        """Gets the built_in of this DocumentProperty.  # noqa: E501
+
+        Gets or sets a value indicating whether the property is built-in or not. If true the property is built-in, if false the property is custom.  # noqa: E501
+
+        :return: The built_in of this DocumentProperty.  # noqa: E501
+        :rtype: bool
+        """
+        return self._built_in
+
+    @built_in.setter
+    def built_in(self, built_in):
+        """Sets the built_in of this DocumentProperty.
+
+        Gets or sets a value indicating whether the property is built-in or not. If true the property is built-in, if false the property is custom.  # noqa: E501
+
+        :param built_in: The built_in of this DocumentProperty.  # noqa: E501
+        :type: bool
+        """
+        self._built_in = built_in
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/info_additional_item.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/info_additional_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/borders_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/borders_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/classification_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/classification_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/html_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/html_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,17 @@
         'images_folder_alias': 'str',
         'metafile_format': 'str',
         'office_math_output_mode': 'str',
         'pretty_format': 'bool',
         'resolve_font_names': 'bool',
         'resource_folder': 'str',
         'resource_folder_alias': 'str',
-        'save_format': 'str',
         'scale_image_to_shape_size': 'bool',
-        'table_width_output_mode': 'str'
+        'table_width_output_mode': 'str',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -142,17 +142,17 @@
         'images_folder_alias': 'ImagesFolderAlias',
         'metafile_format': 'MetafileFormat',
         'office_math_output_mode': 'OfficeMathOutputMode',
         'pretty_format': 'PrettyFormat',
         'resolve_font_names': 'ResolveFontNames',
         'resource_folder': 'ResourceFolder',
         'resource_folder_alias': 'ResourceFolderAlias',
-        'save_format': 'SaveFormat',
         'scale_image_to_shape_size': 'ScaleImageToShapeSize',
-        'table_width_output_mode': 'TableWidthOutputMode'
+        'table_width_output_mode': 'TableWidthOutputMode',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, allow_negative_indent=None, css_class_name_prefix=None, css_style_sheet_file_name=None, css_style_sheet_type=None, document_split_criteria=None, document_split_heading_level=None, encoding=None, export_document_properties=None, export_drop_down_form_field_as_text=None, export_font_resources=None, export_fonts_as_base64=None, export_headers_footers_mode=None, export_images_as_base64=None, export_language_information=None, export_list_labels=None, export_original_url_for_linked_images=None, export_page_margins=None, export_page_setup=None, export_relative_font_size=None, export_roundtrip_information=None, export_text_input_form_field_as_text=None, export_toc_page_numbers=None, export_xhtml_transitional=None, font_resources_subsetting_size_threshold=None, fonts_folder=None, fonts_folder_alias=None, html_version=None, image_resolution=None, images_folder=None, images_folder_alias=None, metafile_format=None, office_math_output_mode=None, pretty_format=None, resolve_font_names=None, resource_folder=None, resource_folder_alias=None, scale_image_to_shape_size=None, table_width_output_mode=None):  # noqa: E501
         """HtmlSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -199,17 +199,17 @@
         self._images_folder_alias = None
         self._metafile_format = None
         self._office_math_output_mode = None
         self._pretty_format = None
         self._resolve_font_names = None
         self._resource_folder = None
         self._resource_folder_alias = None
-        self._save_format = "html"
         self._scale_image_to_shape_size = None
         self._table_width_output_mode = None
+        self._save_format = "html"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -1474,26 +1474,14 @@
 
         :param resource_folder_alias: The resource_folder_alias of this HtmlSaveOptionsData.  # noqa: E501
         :type: str
         """
         self._resource_folder_alias = resource_folder_alias
 
     @property
-    def save_format(self):
-        """Gets the save_format of this HtmlSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this HtmlSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def scale_image_to_shape_size(self):
         """Gets the scale_image_to_shape_size of this HtmlSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether images are scaled by Aspose.Words to the bounding shape size when exporting.  # noqa: E501
 
         :return: The scale_image_to_shape_size of this HtmlSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -1537,14 +1525,26 @@
                 raise ValueError(
                     "Invalid value for `table_width_output_mode` ({0}), must be one of {1}"  # noqa: E501
                     .format(table_width_output_mode, allowed_values))
             self._table_width_output_mode = table_width_output_mode
         else:
             self._table_width_output_mode = allowed_values[int(table_width_output_mode) if six.PY3 else long(table_width_output_mode)]
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this HtmlSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this HtmlSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_fixed_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_fixed_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_link_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comments_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/svg_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/svg_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         'optimize_output': 'bool',
         'page_count': 'int',
         'page_index': 'int',
         'export_embedded_images': 'bool',
         'fit_to_view_port': 'bool',
         'resources_folder': 'str',
         'resources_folder_alias': 'str',
-        'save_format': 'str',
         'show_page_border': 'bool',
-        'text_output_mode': 'str'
+        'text_output_mode': 'str',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -92,17 +92,17 @@
         'optimize_output': 'OptimizeOutput',
         'page_count': 'PageCount',
         'page_index': 'PageIndex',
         'export_embedded_images': 'ExportEmbeddedImages',
         'fit_to_view_port': 'FitToViewPort',
         'resources_folder': 'ResourcesFolder',
         'resources_folder_alias': 'ResourcesFolderAlias',
-        'save_format': 'SaveFormat',
         'show_page_border': 'ShowPageBorder',
-        'text_output_mode': 'TextOutputMode'
+        'text_output_mode': 'TextOutputMode',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, export_embedded_images=None, fit_to_view_port=None, resources_folder=None, resources_folder_alias=None, show_page_border=None, text_output_mode=None):  # noqa: E501
         """SvgSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -124,17 +124,17 @@
         self._optimize_output = None
         self._page_count = None
         self._page_index = None
         self._export_embedded_images = None
         self._fit_to_view_port = None
         self._resources_folder = None
         self._resources_folder_alias = None
-        self._save_format = "svg"
         self._show_page_border = None
         self._text_output_mode = None
+        self._save_format = "svg"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -759,26 +759,14 @@
 
         :param resources_folder_alias: The resources_folder_alias of this SvgSaveOptionsData.  # noqa: E501
         :type: str
         """
         self._resources_folder_alias = resources_folder_alias
 
     @property
-    def save_format(self):
-        """Gets the save_format of this SvgSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this SvgSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def show_page_border(self):
         """Gets the show_page_border of this SvgSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to show or hide page stepper.  # noqa: E501
 
         :return: The show_page_border of this SvgSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -822,14 +810,26 @@
                 raise ValueError(
                     "Invalid value for `text_output_mode` ({0}), must be one of {1}"  # noqa: E501
                     .format(text_output_mode, allowed_values))
             self._text_output_mode = text_output_mode
         else:
             self._text_output_mode = allowed_values[int(text_output_mode) if six.PY3 else long(text_output_mode)]
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this SvgSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this SvgSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_template_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/gif_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/gif_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
+        'use_gdi_emf_renderer': 'bool',
         'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
@@ -103,21 +103,21 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None):  # noqa: E501
         """GifSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -141,17 +141,17 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
+        self._use_gdi_emf_renderer = None
         self._save_format = "gif"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
@@ -205,20 +205,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def allow_embedding_post_script_fonts(self):
         """Gets the allow_embedding_post_script_fonts of this GifSaveOptionsData.  # noqa: E501
 
         Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false..  # noqa: E501
 
@@ -915,36 +915,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this GifSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this GifSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this GifSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this GifSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -981,14 +959,36 @@
 
         :param vertical_resolution: The vertical_resolution of this GifSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :return: The use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this GifSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this GifSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
+
+    @property
     def save_format(self):
         """Gets the save_format of this GifSaveOptionsData.  # noqa: E501
 
         Gets the format of save.  # noqa: E501
 
         :return: The save_format of this GifSaveOptionsData.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/borders_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/borders_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/header_footers_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footers_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xps_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xps_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         'numeral_format': 'str',
         'optimize_output': 'bool',
         'page_count': 'int',
         'page_index': 'int',
         'bookmarks_outline_level': 'int',
         'headings_outline_levels': 'int',
         'outline_options': 'OutlineOptionsData',
-        'save_format': 'str',
-        'use_book_fold_printing_settings': 'bool'
+        'use_book_fold_printing_settings': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -89,16 +89,16 @@
         'numeral_format': 'NumeralFormat',
         'optimize_output': 'OptimizeOutput',
         'page_count': 'PageCount',
         'page_index': 'PageIndex',
         'bookmarks_outline_level': 'BookmarksOutlineLevel',
         'headings_outline_levels': 'HeadingsOutlineLevels',
         'outline_options': 'OutlineOptions',
-        'save_format': 'SaveFormat',
-        'use_book_fold_printing_settings': 'UseBookFoldPrintingSettings'
+        'use_book_fold_printing_settings': 'UseBookFoldPrintingSettings',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, bookmarks_outline_level=None, headings_outline_levels=None, outline_options=None, use_book_fold_printing_settings=None):  # noqa: E501
         """XpsSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -119,16 +119,16 @@
         self._numeral_format = None
         self._optimize_output = None
         self._page_count = None
         self._page_index = None
         self._bookmarks_outline_level = None
         self._headings_outline_levels = None
         self._outline_options = None
-        self._save_format = "xps"
         self._use_book_fold_printing_settings = None
+        self._save_format = "xps"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -727,26 +727,14 @@
 
         :param outline_options: The outline_options of this XpsSaveOptionsData.  # noqa: E501
         :type: OutlineOptionsData
         """
         self._outline_options = outline_options
 
     @property
-    def save_format(self):
-        """Gets the save_format of this XpsSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this XpsSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def use_book_fold_printing_settings(self):
         """Gets the use_book_fold_printing_settings of this XpsSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether the document should be saved using a booklet printing layout.  # noqa: E501
 
         :return: The use_book_fold_printing_settings of this XpsSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -760,14 +748,26 @@
         Gets or sets a value indicating whether the document should be saved using a booklet printing layout.  # noqa: E501
 
         :param use_book_fold_printing_settings: The use_book_fold_printing_settings of this XpsSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_book_fold_printing_settings = use_book_fold_printing_settings
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this XpsSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this XpsSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_level.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,88 +39,88 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
+        'start_at': 'int',
+        'number_style': 'str',
+        'number_format': 'str',
         'alignment': 'str',
-        'font': 'Font',
         'is_legal': 'bool',
-        'linked_style': 'Style',
-        'number_format': 'str',
-        'number_position': 'float',
-        'number_style': 'str',
         'restart_after_level': 'int',
-        'start_at': 'int',
+        'trailing_character': 'str',
+        'font': 'Font',
         'tab_position': 'float',
+        'number_position': 'float',
         'text_position': 'float',
-        'trailing_character': 'str'
+        'linked_style': 'Style'
     }
 
     attribute_map = {
         'link': 'Link',
+        'start_at': 'StartAt',
+        'number_style': 'NumberStyle',
+        'number_format': 'NumberFormat',
         'alignment': 'Alignment',
-        'font': 'Font',
         'is_legal': 'IsLegal',
-        'linked_style': 'LinkedStyle',
-        'number_format': 'NumberFormat',
-        'number_position': 'NumberPosition',
-        'number_style': 'NumberStyle',
         'restart_after_level': 'RestartAfterLevel',
-        'start_at': 'StartAt',
+        'trailing_character': 'TrailingCharacter',
+        'font': 'Font',
         'tab_position': 'TabPosition',
+        'number_position': 'NumberPosition',
         'text_position': 'TextPosition',
-        'trailing_character': 'TrailingCharacter'
+        'linked_style': 'LinkedStyle'
     }
 
-    def __init__(self, link=None, alignment=None, font=None, is_legal=None, linked_style=None, number_format=None, number_position=None, number_style=None, restart_after_level=None, start_at=None, tab_position=None, text_position=None, trailing_character=None):  # noqa: E501
+    def __init__(self, link=None, start_at=None, number_style=None, number_format=None, alignment=None, is_legal=None, restart_after_level=None, trailing_character=None, font=None, tab_position=None, number_position=None, text_position=None, linked_style=None):  # noqa: E501
         """ListLevel - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
+        self._start_at = None
+        self._number_style = None
+        self._number_format = None
         self._alignment = None
-        self._font = None
         self._is_legal = None
-        self._linked_style = None
-        self._number_format = None
-        self._number_position = None
-        self._number_style = None
         self._restart_after_level = None
-        self._start_at = None
+        self._trailing_character = None
+        self._font = None
         self._tab_position = None
+        self._number_position = None
         self._text_position = None
-        self._trailing_character = None
+        self._linked_style = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
+        if start_at is not None:
+            self.start_at = start_at
+        if number_style is not None:
+            self.number_style = number_style
+        if number_format is not None:
+            self.number_format = number_format
         if alignment is not None:
             self.alignment = alignment
-        if font is not None:
-            self.font = font
         if is_legal is not None:
             self.is_legal = is_legal
-        if linked_style is not None:
-            self.linked_style = linked_style
-        if number_format is not None:
-            self.number_format = number_format
-        if number_position is not None:
-            self.number_position = number_position
-        if number_style is not None:
-            self.number_style = number_style
         if restart_after_level is not None:
             self.restart_after_level = restart_after_level
-        if start_at is not None:
-            self.start_at = start_at
+        if trailing_character is not None:
+            self.trailing_character = trailing_character
+        if font is not None:
+            self.font = font
         if tab_position is not None:
             self.tab_position = tab_position
+        if number_position is not None:
+            self.number_position = number_position
         if text_position is not None:
             self.text_position = text_position
-        if trailing_character is not None:
-            self.trailing_character = trailing_character
+        if linked_style is not None:
+            self.linked_style = linked_style
 
     @property
     def link(self):
         """Gets the link of this ListLevel.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -137,108 +137,64 @@
 
         :param link: The link of this ListLevel.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def alignment(self):
-        """Gets the alignment of this ListLevel.  # noqa: E501
-
-        Gets or sets the justification of the actual number of the list item.  # noqa: E501
-
-        :return: The alignment of this ListLevel.  # noqa: E501
-        :rtype: str
-        """
-        return self._alignment
-
-    @alignment.setter
-    def alignment(self, alignment):
-        """Sets the alignment of this ListLevel.
-
-        Gets or sets the justification of the actual number of the list item.  # noqa: E501
-
-        :param alignment: The alignment of this ListLevel.  # noqa: E501
-        :type: str
-        """
-        allowed_values = ["Left", "Center", "Right"]  # noqa: E501
-        if not alignment.isdigit():
-            if alignment not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `alignment` ({0}), must be one of {1}"  # noqa: E501
-                    .format(alignment, allowed_values))
-            self._alignment = alignment
-        else:
-            self._alignment = allowed_values[int(alignment) if six.PY3 else long(alignment)]
-
-    @property
-    def font(self):
-        """Gets the font of this ListLevel.  # noqa: E501
-
-        Gets or sets character formatting used for the list label.  # noqa: E501
-
-        :return: The font of this ListLevel.  # noqa: E501
-        :rtype: Font
-        """
-        return self._font
-
-    @font.setter
-    def font(self, font):
-        """Sets the font of this ListLevel.
-
-        Gets or sets character formatting used for the list label.  # noqa: E501
-
-        :param font: The font of this ListLevel.  # noqa: E501
-        :type: Font
-        """
-        self._font = font
-
-    @property
-    def is_legal(self):
-        """Gets the is_legal of this ListLevel.  # noqa: E501
+    def start_at(self):
+        """Gets the start_at of this ListLevel.  # noqa: E501
 
-        Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style.  # noqa: E501
+        Gets or sets the starting number for this list level.  # noqa: E501
 
-        :return: The is_legal of this ListLevel.  # noqa: E501
-        :rtype: bool
+        :return: The start_at of this ListLevel.  # noqa: E501
+        :rtype: int
         """
-        return self._is_legal
+        return self._start_at
 
-    @is_legal.setter
-    def is_legal(self, is_legal):
-        """Sets the is_legal of this ListLevel.
+    @start_at.setter
+    def start_at(self, start_at):
+        """Sets the start_at of this ListLevel.
 
-        Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style.  # noqa: E501
+        Gets or sets the starting number for this list level.  # noqa: E501
 
-        :param is_legal: The is_legal of this ListLevel.  # noqa: E501
-        :type: bool
+        :param start_at: The start_at of this ListLevel.  # noqa: E501
+        :type: int
         """
-        self._is_legal = is_legal
+        self._start_at = start_at
 
     @property
-    def linked_style(self):
-        """Gets the linked_style of this ListLevel.  # noqa: E501
+    def number_style(self):
+        """Gets the number_style of this ListLevel.  # noqa: E501
 
-        Gets or sets the paragraph style that is linked to this list level.  # noqa: E501
+        Gets or sets the number style for this list level.  # noqa: E501
 
-        :return: The linked_style of this ListLevel.  # noqa: E501
-        :rtype: Style
+        :return: The number_style of this ListLevel.  # noqa: E501
+        :rtype: str
         """
-        return self._linked_style
+        return self._number_style
 
-    @linked_style.setter
-    def linked_style(self, linked_style):
-        """Sets the linked_style of this ListLevel.
+    @number_style.setter
+    def number_style(self, number_style):
+        """Sets the number_style of this ListLevel.
 
-        Gets or sets the paragraph style that is linked to this list level.  # noqa: E501
+        Gets or sets the number style for this list level.  # noqa: E501
 
-        :param linked_style: The linked_style of this ListLevel.  # noqa: E501
-        :type: Style
+        :param number_style: The number_style of this ListLevel.  # noqa: E501
+        :type: str
         """
-        self._linked_style = linked_style
+        allowed_values = ["Arabic", "UppercaseRoman", "LowercaseRoman", "UppercaseLetter", "LowercaseLetter", "Ordinal", "Number", "OrdinalText", "Hex", "ChicagoManual", "Kanji", "KanjiDigit", "AiueoHalfWidth", "IrohaHalfWidth", "ArabicFullWidth", "ArabicHalfWidth", "KanjiTraditional", "KanjiTraditional2", "NumberInCircle", "DecimalFullWidth", "Aiueo", "Iroha", "LeadingZero", "Bullet", "Ganada", "Chosung", "GB1", "GB2", "GB3", "GB4", "Zodiac1", "Zodiac2", "Zodiac3", "TradChinNum1", "TradChinNum2", "TradChinNum3", "TradChinNum4", "SimpChinNum1", "SimpChinNum2", "SimpChinNum3", "SimpChinNum4", "HanjaRead", "HanjaReadDigit", "Hangul", "Hanja", "Hebrew1", "Arabic1", "Hebrew2", "Arabic2", "HindiLetter1", "HindiLetter2", "HindiArabic", "HindiCardinalText", "ThaiLetter", "ThaiArabic", "ThaiCardinalText", "VietCardinalText", "NumberInDash", "LowercaseRussian", "UppercaseRussian", "None", "Custom"]  # noqa: E501
+        if not number_style.isdigit():
+            if number_style not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `number_style` ({0}), must be one of {1}"  # noqa: E501
+                    .format(number_style, allowed_values))
+            self._number_style = number_style
+        else:
+            self._number_style = allowed_values[int(number_style) if six.PY3 else long(number_style)]
 
     @property
     def number_format(self):
         """Gets the number_format of this ListLevel.  # noqa: E501
 
         Gets or sets the number format for the list level.  # noqa: E501
 
@@ -255,64 +211,64 @@
 
         :param number_format: The number_format of this ListLevel.  # noqa: E501
         :type: str
         """
         self._number_format = number_format
 
     @property
-    def number_position(self):
-        """Gets the number_position of this ListLevel.  # noqa: E501
+    def alignment(self):
+        """Gets the alignment of this ListLevel.  # noqa: E501
 
-        Gets or sets the position (in points) of the number or bullet for the list level.  # noqa: E501
+        Gets or sets the justification of the actual number of the list item.  # noqa: E501
 
-        :return: The number_position of this ListLevel.  # noqa: E501
-        :rtype: float
+        :return: The alignment of this ListLevel.  # noqa: E501
+        :rtype: str
         """
-        return self._number_position
+        return self._alignment
 
-    @number_position.setter
-    def number_position(self, number_position):
-        """Sets the number_position of this ListLevel.
+    @alignment.setter
+    def alignment(self, alignment):
+        """Sets the alignment of this ListLevel.
 
-        Gets or sets the position (in points) of the number or bullet for the list level.  # noqa: E501
+        Gets or sets the justification of the actual number of the list item.  # noqa: E501
 
-        :param number_position: The number_position of this ListLevel.  # noqa: E501
-        :type: float
+        :param alignment: The alignment of this ListLevel.  # noqa: E501
+        :type: str
         """
-        self._number_position = number_position
+        allowed_values = ["Left", "Center", "Right"]  # noqa: E501
+        if not alignment.isdigit():
+            if alignment not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `alignment` ({0}), must be one of {1}"  # noqa: E501
+                    .format(alignment, allowed_values))
+            self._alignment = alignment
+        else:
+            self._alignment = allowed_values[int(alignment) if six.PY3 else long(alignment)]
 
     @property
-    def number_style(self):
-        """Gets the number_style of this ListLevel.  # noqa: E501
+    def is_legal(self):
+        """Gets the is_legal of this ListLevel.  # noqa: E501
 
-        Gets or sets the number style for this list level.  # noqa: E501
+        Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style.  # noqa: E501
 
-        :return: The number_style of this ListLevel.  # noqa: E501
-        :rtype: str
+        :return: The is_legal of this ListLevel.  # noqa: E501
+        :rtype: bool
         """
-        return self._number_style
+        return self._is_legal
 
-    @number_style.setter
-    def number_style(self, number_style):
-        """Sets the number_style of this ListLevel.
+    @is_legal.setter
+    def is_legal(self, is_legal):
+        """Sets the is_legal of this ListLevel.
 
-        Gets or sets the number style for this list level.  # noqa: E501
+        Gets or sets a value indicating whether the level turns all inherited numbers to Arabic, false if it preserves their number style.  # noqa: E501
 
-        :param number_style: The number_style of this ListLevel.  # noqa: E501
-        :type: str
+        :param is_legal: The is_legal of this ListLevel.  # noqa: E501
+        :type: bool
         """
-        allowed_values = ["Arabic", "UppercaseRoman", "LowercaseRoman", "UppercaseLetter", "LowercaseLetter", "Ordinal", "Number", "OrdinalText", "Hex", "ChicagoManual", "Kanji", "KanjiDigit", "AiueoHalfWidth", "IrohaHalfWidth", "ArabicFullWidth", "ArabicHalfWidth", "KanjiTraditional", "KanjiTraditional2", "NumberInCircle", "DecimalFullWidth", "Aiueo", "Iroha", "LeadingZero", "Bullet", "Ganada", "Chosung", "GB1", "GB2", "GB3", "GB4", "Zodiac1", "Zodiac2", "Zodiac3", "TradChinNum1", "TradChinNum2", "TradChinNum3", "TradChinNum4", "SimpChinNum1", "SimpChinNum2", "SimpChinNum3", "SimpChinNum4", "HanjaRead", "HanjaReadDigit", "Hangul", "Hanja", "Hebrew1", "Arabic1", "Hebrew2", "Arabic2", "HindiLetter1", "HindiLetter2", "HindiArabic", "HindiCardinalText", "ThaiLetter", "ThaiArabic", "ThaiCardinalText", "VietCardinalText", "NumberInDash", "LowercaseRussian", "UppercaseRussian", "None", "Custom"]  # noqa: E501
-        if not number_style.isdigit():
-            if number_style not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `number_style` ({0}), must be one of {1}"  # noqa: E501
-                    .format(number_style, allowed_values))
-            self._number_style = number_style
-        else:
-            self._number_style = allowed_values[int(number_style) if six.PY3 else long(number_style)]
+        self._is_legal = is_legal
 
     @property
     def restart_after_level(self):
         """Gets the restart_after_level of this ListLevel.  # noqa: E501
 
         Gets or sets the list level, that must appear before the specified list level restarts numbering.  # noqa: E501
 
@@ -329,34 +285,64 @@
 
         :param restart_after_level: The restart_after_level of this ListLevel.  # noqa: E501
         :type: int
         """
         self._restart_after_level = restart_after_level
 
     @property
-    def start_at(self):
-        """Gets the start_at of this ListLevel.  # noqa: E501
+    def trailing_character(self):
+        """Gets the trailing_character of this ListLevel.  # noqa: E501
 
-        Gets or sets the starting number for this list level.  # noqa: E501
+        Gets or sets the character inserted after the number for the list level.  # noqa: E501
 
-        :return: The start_at of this ListLevel.  # noqa: E501
-        :rtype: int
+        :return: The trailing_character of this ListLevel.  # noqa: E501
+        :rtype: str
         """
-        return self._start_at
+        return self._trailing_character
 
-    @start_at.setter
-    def start_at(self, start_at):
-        """Sets the start_at of this ListLevel.
+    @trailing_character.setter
+    def trailing_character(self, trailing_character):
+        """Sets the trailing_character of this ListLevel.
 
-        Gets or sets the starting number for this list level.  # noqa: E501
+        Gets or sets the character inserted after the number for the list level.  # noqa: E501
 
-        :param start_at: The start_at of this ListLevel.  # noqa: E501
-        :type: int
+        :param trailing_character: The trailing_character of this ListLevel.  # noqa: E501
+        :type: str
         """
-        self._start_at = start_at
+        allowed_values = ["Tab", "Space", "Nothing"]  # noqa: E501
+        if not trailing_character.isdigit():
+            if trailing_character not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `trailing_character` ({0}), must be one of {1}"  # noqa: E501
+                    .format(trailing_character, allowed_values))
+            self._trailing_character = trailing_character
+        else:
+            self._trailing_character = allowed_values[int(trailing_character) if six.PY3 else long(trailing_character)]
+
+    @property
+    def font(self):
+        """Gets the font of this ListLevel.  # noqa: E501
+
+        Gets or sets character formatting used for the list label.  # noqa: E501
+
+        :return: The font of this ListLevel.  # noqa: E501
+        :rtype: Font
+        """
+        return self._font
+
+    @font.setter
+    def font(self, font):
+        """Sets the font of this ListLevel.
+
+        Gets or sets character formatting used for the list label.  # noqa: E501
+
+        :param font: The font of this ListLevel.  # noqa: E501
+        :type: Font
+        """
+        self._font = font
 
     @property
     def tab_position(self):
         """Gets the tab_position of this ListLevel.  # noqa: E501
 
         Gets or sets the tab position (in points) for the list level.  # noqa: E501
 
@@ -373,14 +359,36 @@
 
         :param tab_position: The tab_position of this ListLevel.  # noqa: E501
         :type: float
         """
         self._tab_position = tab_position
 
     @property
+    def number_position(self):
+        """Gets the number_position of this ListLevel.  # noqa: E501
+
+        Gets or sets the position (in points) of the number or bullet for the list level.  # noqa: E501
+
+        :return: The number_position of this ListLevel.  # noqa: E501
+        :rtype: float
+        """
+        return self._number_position
+
+    @number_position.setter
+    def number_position(self, number_position):
+        """Sets the number_position of this ListLevel.
+
+        Gets or sets the position (in points) of the number or bullet for the list level.  # noqa: E501
+
+        :param number_position: The number_position of this ListLevel.  # noqa: E501
+        :type: float
+        """
+        self._number_position = number_position
+
+    @property
     def text_position(self):
         """Gets the text_position of this ListLevel.  # noqa: E501
 
         Gets or sets the position (in points) for the second line of wrapping text for the list level.  # noqa: E501
 
         :return: The text_position of this ListLevel.  # noqa: E501
         :rtype: float
@@ -395,42 +403,34 @@
 
         :param text_position: The text_position of this ListLevel.  # noqa: E501
         :type: float
         """
         self._text_position = text_position
 
     @property
-    def trailing_character(self):
-        """Gets the trailing_character of this ListLevel.  # noqa: E501
+    def linked_style(self):
+        """Gets the linked_style of this ListLevel.  # noqa: E501
 
-        Gets or sets the character inserted after the number for the list level.  # noqa: E501
+        Gets or sets the paragraph style that is linked to this list level.  # noqa: E501
 
-        :return: The trailing_character of this ListLevel.  # noqa: E501
-        :rtype: str
+        :return: The linked_style of this ListLevel.  # noqa: E501
+        :rtype: Style
         """
-        return self._trailing_character
+        return self._linked_style
 
-    @trailing_character.setter
-    def trailing_character(self, trailing_character):
-        """Sets the trailing_character of this ListLevel.
+    @linked_style.setter
+    def linked_style(self, linked_style):
+        """Sets the linked_style of this ListLevel.
 
-        Gets or sets the character inserted after the number for the list level.  # noqa: E501
+        Gets or sets the paragraph style that is linked to this list level.  # noqa: E501
 
-        :param trailing_character: The trailing_character of this ListLevel.  # noqa: E501
-        :type: str
+        :param linked_style: The linked_style of this ListLevel.  # noqa: E501
+        :type: Style
         """
-        allowed_values = ["Tab", "Space", "Nothing"]  # noqa: E501
-        if not trailing_character.isdigit():
-            if trailing_character not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `trailing_character` ({0}), must be one of {1}"  # noqa: E501
-                    .format(trailing_character, allowed_values))
-            self._trailing_character = trailing_character
-        else:
-            self._trailing_character = allowed_values[int(trailing_character) if six.PY3 else long(trailing_character)]
+        self._linked_style = linked_style
 
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/run_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/run_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,20 +80,20 @@
         'image_compression': 'str',
         'interpolate_images': 'bool',
         'open_hyperlinks_in_new_window': 'bool',
         'outline_options': 'OutlineOptionsData',
         'page_mode': 'str',
         'preblend_images': 'bool',
         'preserve_form_fields': 'bool',
-        'save_format': 'str',
         'text_compression': 'str',
         'use_book_fold_printing_settings': 'bool',
         'use_core_fonts': 'bool',
         'zoom_behavior': 'str',
-        'zoom_factor': 'int'
+        'zoom_factor': 'int',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -131,20 +131,20 @@
         'image_compression': 'ImageCompression',
         'interpolate_images': 'InterpolateImages',
         'open_hyperlinks_in_new_window': 'OpenHyperlinksInNewWindow',
         'outline_options': 'OutlineOptions',
         'page_mode': 'PageMode',
         'preblend_images': 'PreblendImages',
         'preserve_form_fields': 'PreserveFormFields',
-        'save_format': 'SaveFormat',
         'text_compression': 'TextCompression',
         'use_book_fold_printing_settings': 'UseBookFoldPrintingSettings',
         'use_core_fonts': 'UseCoreFonts',
         'zoom_behavior': 'ZoomBehavior',
-        'zoom_factor': 'ZoomFactor'
+        'zoom_factor': 'ZoomFactor',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, cache_background_graphics=None, compliance=None, create_note_hyperlinks=None, custom_properties_export=None, digital_signature_details=None, display_doc_title=None, downsample_options=None, embed_attachments=None, embed_full_fonts=None, encryption_details=None, export_document_structure=None, export_language_to_span_tag=None, font_embedding_mode=None, header_footer_bookmarks_export_mode=None, image_color_space_export_mode=None, image_compression=None, interpolate_images=None, open_hyperlinks_in_new_window=None, outline_options=None, page_mode=None, preblend_images=None, preserve_form_fields=None, text_compression=None, use_book_fold_printing_settings=None, use_core_fonts=None, zoom_behavior=None, zoom_factor=None):  # noqa: E501
         """PdfSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -184,20 +184,20 @@
         self._image_compression = None
         self._interpolate_images = None
         self._open_hyperlinks_in_new_window = None
         self._outline_options = None
         self._page_mode = None
         self._preblend_images = None
         self._preserve_form_fields = None
-        self._save_format = "pdf"
         self._text_compression = None
         self._use_book_fold_printing_settings = None
         self._use_core_fonts = None
         self._zoom_behavior = None
         self._zoom_factor = None
+        self._save_format = "pdf"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -1308,26 +1308,14 @@
 
         :param preserve_form_fields: The preserve_form_fields of this PdfSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._preserve_form_fields = preserve_form_fields
 
     @property
-    def save_format(self):
-        """Gets the save_format of this PdfSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this PdfSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def text_compression(self):
         """Gets the text_compression of this PdfSaveOptionsData.  # noqa: E501
 
         Gets or sets the compression type to be used for all textual content in the document.  # noqa: E501
 
         :return: The text_compression of this PdfSaveOptionsData.  # noqa: E501
         :rtype: str
@@ -1445,14 +1433,26 @@
         Gets or sets the zoom factor (in percentages) for a document.  # noqa: E501
 
         :param zoom_factor: The zoom_factor of this PdfSaveOptionsData.  # noqa: E501
         :type: int
         """
         self._zoom_factor = zoom_factor
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this PdfSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this PdfSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style_copy.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style_copy.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,80 +40,80 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
+        'render_links': 'list[WordsApiLink]',
+        'width': 'float',
         'height': 'float',
-        'image_data_link': 'WordsApiLink',
-        'left': 'float',
         'ole_data_link': 'WordsApiLink',
+        'image_data_link': 'WordsApiLink',
         'relative_horizontal_position': 'str',
+        'left': 'float',
         'relative_vertical_position': 'str',
-        'render_links': 'list[WordsApiLink]',
         'top': 'float',
-        'width': 'float',
         'wrap_type': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
+        'render_links': 'RenderLinks',
+        'width': 'Width',
         'height': 'Height',
-        'image_data_link': 'ImageDataLink',
-        'left': 'Left',
         'ole_data_link': 'OleDataLink',
+        'image_data_link': 'ImageDataLink',
         'relative_horizontal_position': 'RelativeHorizontalPosition',
+        'left': 'Left',
         'relative_vertical_position': 'RelativeVerticalPosition',
-        'render_links': 'RenderLinks',
         'top': 'Top',
-        'width': 'Width',
         'wrap_type': 'WrapType'
     }
 
-    def __init__(self, link=None, node_id=None, height=None, image_data_link=None, left=None, ole_data_link=None, relative_horizontal_position=None, relative_vertical_position=None, render_links=None, top=None, width=None, wrap_type=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, render_links=None, width=None, height=None, ole_data_link=None, image_data_link=None, relative_horizontal_position=None, left=None, relative_vertical_position=None, top=None, wrap_type=None):  # noqa: E501
         """DrawingObject - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
+        self._render_links = None
+        self._width = None
         self._height = None
-        self._image_data_link = None
-        self._left = None
         self._ole_data_link = None
+        self._image_data_link = None
         self._relative_horizontal_position = None
+        self._left = None
         self._relative_vertical_position = None
-        self._render_links = None
         self._top = None
-        self._width = None
         self._wrap_type = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
+        if render_links is not None:
+            self.render_links = render_links
+        if width is not None:
+            self.width = width
         if height is not None:
             self.height = height
-        if image_data_link is not None:
-            self.image_data_link = image_data_link
-        if left is not None:
-            self.left = left
         if ole_data_link is not None:
             self.ole_data_link = ole_data_link
+        if image_data_link is not None:
+            self.image_data_link = image_data_link
         if relative_horizontal_position is not None:
             self.relative_horizontal_position = relative_horizontal_position
+        if left is not None:
+            self.left = left
         if relative_vertical_position is not None:
             self.relative_vertical_position = relative_vertical_position
-        if render_links is not None:
-            self.render_links = render_links
         if top is not None:
             self.top = top
-        if width is not None:
-            self.width = width
         if wrap_type is not None:
             self.wrap_type = wrap_type
 
     @property
     def link(self):
         """Gets the link of this DrawingObject.  # noqa: E501
 
@@ -154,78 +154,78 @@
 
         :param node_id: The node_id of this DrawingObject.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def height(self):
-        """Gets the height of this DrawingObject.  # noqa: E501
+    def render_links(self):
+        """Gets the render_links of this DrawingObject.  # noqa: E501
 
-        Gets or sets the height of the DrawingObject in points.  # noqa: E501
+        Gets or sets the list of links that originate from this DrawingObjectDto.  # noqa: E501
 
-        :return: The height of this DrawingObject.  # noqa: E501
-        :rtype: float
+        :return: The render_links of this DrawingObject.  # noqa: E501
+        :rtype: list[WordsApiLink]
         """
-        return self._height
+        return self._render_links
 
-    @height.setter
-    def height(self, height):
-        """Sets the height of this DrawingObject.
+    @render_links.setter
+    def render_links(self, render_links):
+        """Sets the render_links of this DrawingObject.
 
-        Gets or sets the height of the DrawingObject in points.  # noqa: E501
+        Gets or sets the list of links that originate from this DrawingObjectDto.  # noqa: E501
 
-        :param height: The height of this DrawingObject.  # noqa: E501
-        :type: float
+        :param render_links: The render_links of this DrawingObject.  # noqa: E501
+        :type: list[WordsApiLink]
         """
-        self._height = height
+        self._render_links = render_links
 
     @property
-    def image_data_link(self):
-        """Gets the image_data_link of this DrawingObject.  # noqa: E501
+    def width(self):
+        """Gets the width of this DrawingObject.  # noqa: E501
 
-        Gets or sets the link to image data. Can be null if shape does not have an image.  # noqa: E501
+        Gets or sets the width of the DrawingObjects in points.  # noqa: E501
 
-        :return: The image_data_link of this DrawingObject.  # noqa: E501
-        :rtype: WordsApiLink
+        :return: The width of this DrawingObject.  # noqa: E501
+        :rtype: float
         """
-        return self._image_data_link
+        return self._width
 
-    @image_data_link.setter
-    def image_data_link(self, image_data_link):
-        """Sets the image_data_link of this DrawingObject.
+    @width.setter
+    def width(self, width):
+        """Sets the width of this DrawingObject.
 
-        Gets or sets the link to image data. Can be null if shape does not have an image.  # noqa: E501
+        Gets or sets the width of the DrawingObjects in points.  # noqa: E501
 
-        :param image_data_link: The image_data_link of this DrawingObject.  # noqa: E501
-        :type: WordsApiLink
+        :param width: The width of this DrawingObject.  # noqa: E501
+        :type: float
         """
-        self._image_data_link = image_data_link
+        self._width = width
 
     @property
-    def left(self):
-        """Gets the left of this DrawingObject.  # noqa: E501
+    def height(self):
+        """Gets the height of this DrawingObject.  # noqa: E501
 
-        Gets or sets the distance in points from the origin to the left side of the image.  # noqa: E501
+        Gets or sets the height of the DrawingObject in points.  # noqa: E501
 
-        :return: The left of this DrawingObject.  # noqa: E501
+        :return: The height of this DrawingObject.  # noqa: E501
         :rtype: float
         """
-        return self._left
+        return self._height
 
-    @left.setter
-    def left(self, left):
-        """Sets the left of this DrawingObject.
+    @height.setter
+    def height(self, height):
+        """Sets the height of this DrawingObject.
 
-        Gets or sets the distance in points from the origin to the left side of the image.  # noqa: E501
+        Gets or sets the height of the DrawingObject in points.  # noqa: E501
 
-        :param left: The left of this DrawingObject.  # noqa: E501
+        :param height: The height of this DrawingObject.  # noqa: E501
         :type: float
         """
-        self._left = left
+        self._height = height
 
     @property
     def ole_data_link(self):
         """Gets the ole_data_link of this DrawingObject.  # noqa: E501
 
         Gets or sets the link to OLE object. Can be null if shape does not have OLE data.  # noqa: E501
 
@@ -242,14 +242,36 @@
 
         :param ole_data_link: The ole_data_link of this DrawingObject.  # noqa: E501
         :type: WordsApiLink
         """
         self._ole_data_link = ole_data_link
 
     @property
+    def image_data_link(self):
+        """Gets the image_data_link of this DrawingObject.  # noqa: E501
+
+        Gets or sets the link to image data. Can be null if shape does not have an image.  # noqa: E501
+
+        :return: The image_data_link of this DrawingObject.  # noqa: E501
+        :rtype: WordsApiLink
+        """
+        return self._image_data_link
+
+    @image_data_link.setter
+    def image_data_link(self, image_data_link):
+        """Sets the image_data_link of this DrawingObject.
+
+        Gets or sets the link to image data. Can be null if shape does not have an image.  # noqa: E501
+
+        :param image_data_link: The image_data_link of this DrawingObject.  # noqa: E501
+        :type: WordsApiLink
+        """
+        self._image_data_link = image_data_link
+
+    @property
     def relative_horizontal_position(self):
         """Gets the relative_horizontal_position of this DrawingObject.  # noqa: E501
 
         Gets or sets the relative horizontal position, from which the distance to the image is measured.  # noqa: E501
 
         :return: The relative_horizontal_position of this DrawingObject.  # noqa: E501
         :rtype: str
@@ -272,14 +294,36 @@
                     "Invalid value for `relative_horizontal_position` ({0}), must be one of {1}"  # noqa: E501
                     .format(relative_horizontal_position, allowed_values))
             self._relative_horizontal_position = relative_horizontal_position
         else:
             self._relative_horizontal_position = allowed_values[int(relative_horizontal_position) if six.PY3 else long(relative_horizontal_position)]
 
     @property
+    def left(self):
+        """Gets the left of this DrawingObject.  # noqa: E501
+
+        Gets or sets the distance in points from the origin to the left side of the image.  # noqa: E501
+
+        :return: The left of this DrawingObject.  # noqa: E501
+        :rtype: float
+        """
+        return self._left
+
+    @left.setter
+    def left(self, left):
+        """Sets the left of this DrawingObject.
+
+        Gets or sets the distance in points from the origin to the left side of the image.  # noqa: E501
+
+        :param left: The left of this DrawingObject.  # noqa: E501
+        :type: float
+        """
+        self._left = left
+
+    @property
     def relative_vertical_position(self):
         """Gets the relative_vertical_position of this DrawingObject.  # noqa: E501
 
         Gets or sets the relative vertical position, from which the distance to the image is measured.  # noqa: E501
 
         :return: The relative_vertical_position of this DrawingObject.  # noqa: E501
         :rtype: str
@@ -302,36 +346,14 @@
                     "Invalid value for `relative_vertical_position` ({0}), must be one of {1}"  # noqa: E501
                     .format(relative_vertical_position, allowed_values))
             self._relative_vertical_position = relative_vertical_position
         else:
             self._relative_vertical_position = allowed_values[int(relative_vertical_position) if six.PY3 else long(relative_vertical_position)]
 
     @property
-    def render_links(self):
-        """Gets the render_links of this DrawingObject.  # noqa: E501
-
-        Gets or sets the list of links that originate from this DrawingObjectDto.  # noqa: E501
-
-        :return: The render_links of this DrawingObject.  # noqa: E501
-        :rtype: list[WordsApiLink]
-        """
-        return self._render_links
-
-    @render_links.setter
-    def render_links(self, render_links):
-        """Sets the render_links of this DrawingObject.
-
-        Gets or sets the list of links that originate from this DrawingObjectDto.  # noqa: E501
-
-        :param render_links: The render_links of this DrawingObject.  # noqa: E501
-        :type: list[WordsApiLink]
-        """
-        self._render_links = render_links
-
-    @property
     def top(self):
         """Gets the top of this DrawingObject.  # noqa: E501
 
         Gets or sets the distance in points from the origin to the top side of the image.  # noqa: E501
 
         :return: The top of this DrawingObject.  # noqa: E501
         :rtype: float
@@ -346,36 +368,14 @@
 
         :param top: The top of this DrawingObject.  # noqa: E501
         :type: float
         """
         self._top = top
 
     @property
-    def width(self):
-        """Gets the width of this DrawingObject.  # noqa: E501
-
-        Gets or sets the width of the DrawingObjects in points.  # noqa: E501
-
-        :return: The width of this DrawingObject.  # noqa: E501
-        :rtype: float
-        """
-        return self._width
-
-    @width.setter
-    def width(self, width):
-        """Sets the width of this DrawingObject.
-
-        Gets or sets the width of the DrawingObjects in points.  # noqa: E501
-
-        :param width: The width of this DrawingObject.  # noqa: E501
-        :type: float
-        """
-        self._width = width
-
-    @property
     def wrap_type(self):
         """Gets the wrap_type of this DrawingObject.  # noqa: E501
 
         Gets or sets the option that controls how to wrap text around the image.  # noqa: E501
 
         :return: The wrap_type of this DrawingObject.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/revisions_modification_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/revisions_modification_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/info_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/info_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_link_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/style_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/png_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/png_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
+        'use_gdi_emf_renderer': 'bool',
         'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
@@ -103,21 +103,21 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None):  # noqa: E501
         """PngSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -141,17 +141,17 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
+        self._use_gdi_emf_renderer = None
         self._save_format = "png"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
@@ -205,20 +205,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def allow_embedding_post_script_fonts(self):
         """Gets the allow_embedding_post_script_fonts of this PngSaveOptionsData.  # noqa: E501
 
         Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false..  # noqa: E501
 
@@ -915,36 +915,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this PngSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this PngSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this PngSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this PngSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -981,14 +959,36 @@
 
         :param vertical_resolution: The vertical_resolution of this PngSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :return: The use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this PngSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this PngSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
+
+    @property
     def save_format(self):
         """Gets the save_format of this PngSaveOptionsData.  # noqa: E501
 
         Gets the format of save.  # noqa: E501
 
         :return: The save_format of this PngSaveOptionsData.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_text_input.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_text_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,97 +40,97 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'calculate_on_exit': 'bool',
+        'name': 'str',
         'enabled': 'bool',
-        'entry_macro': 'str',
-        'exit_macro': 'str',
+        'status_text': 'str',
+        'own_status': 'bool',
         'help_text': 'str',
-        'name': 'str',
         'own_help': 'bool',
-        'own_status': 'bool',
-        'status_text': 'str',
-        'max_length': 'int',
-        'text_input_default': 'str',
+        'calculate_on_exit': 'bool',
+        'entry_macro': 'str',
+        'exit_macro': 'str',
         'text_input_format': 'str',
-        'text_input_type': 'str'
+        'text_input_type': 'str',
+        'text_input_default': 'str',
+        'max_length': 'int'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'calculate_on_exit': 'CalculateOnExit',
+        'name': 'Name',
         'enabled': 'Enabled',
-        'entry_macro': 'EntryMacro',
-        'exit_macro': 'ExitMacro',
+        'status_text': 'StatusText',
+        'own_status': 'OwnStatus',
         'help_text': 'HelpText',
-        'name': 'Name',
         'own_help': 'OwnHelp',
-        'own_status': 'OwnStatus',
-        'status_text': 'StatusText',
-        'max_length': 'MaxLength',
-        'text_input_default': 'TextInputDefault',
+        'calculate_on_exit': 'CalculateOnExit',
+        'entry_macro': 'EntryMacro',
+        'exit_macro': 'ExitMacro',
         'text_input_format': 'TextInputFormat',
-        'text_input_type': 'TextInputType'
+        'text_input_type': 'TextInputType',
+        'text_input_default': 'TextInputDefault',
+        'max_length': 'MaxLength'
     }
 
-    def __init__(self, link=None, node_id=None, calculate_on_exit=None, enabled=None, entry_macro=None, exit_macro=None, help_text=None, name=None, own_help=None, own_status=None, status_text=None, max_length=None, text_input_default=None, text_input_format=None, text_input_type=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, name=None, enabled=None, status_text=None, own_status=None, help_text=None, own_help=None, calculate_on_exit=None, entry_macro=None, exit_macro=None, text_input_format=None, text_input_type=None, text_input_default=None, max_length=None):  # noqa: E501
         """FormFieldTextInput - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._calculate_on_exit = None
+        self._name = None
         self._enabled = None
-        self._entry_macro = None
-        self._exit_macro = None
+        self._status_text = None
+        self._own_status = None
         self._help_text = None
-        self._name = None
         self._own_help = None
-        self._own_status = None
-        self._status_text = None
-        self._max_length = None
-        self._text_input_default = None
+        self._calculate_on_exit = None
+        self._entry_macro = None
+        self._exit_macro = None
         self._text_input_format = None
         self._text_input_type = None
+        self._text_input_default = None
+        self._max_length = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if calculate_on_exit is not None:
-            self.calculate_on_exit = calculate_on_exit
+        if name is not None:
+            self.name = name
         if enabled is not None:
             self.enabled = enabled
-        if entry_macro is not None:
-            self.entry_macro = entry_macro
-        if exit_macro is not None:
-            self.exit_macro = exit_macro
+        if status_text is not None:
+            self.status_text = status_text
+        if own_status is not None:
+            self.own_status = own_status
         if help_text is not None:
             self.help_text = help_text
-        if name is not None:
-            self.name = name
         if own_help is not None:
             self.own_help = own_help
-        if own_status is not None:
-            self.own_status = own_status
-        if status_text is not None:
-            self.status_text = status_text
-        if max_length is not None:
-            self.max_length = max_length
-        if text_input_default is not None:
-            self.text_input_default = text_input_default
+        if calculate_on_exit is not None:
+            self.calculate_on_exit = calculate_on_exit
+        if entry_macro is not None:
+            self.entry_macro = entry_macro
+        if exit_macro is not None:
+            self.exit_macro = exit_macro
         if text_input_format is not None:
             self.text_input_format = text_input_format
         if text_input_type is not None:
             self.text_input_type = text_input_type
+        if text_input_default is not None:
+            self.text_input_default = text_input_default
+        if max_length is not None:
+            self.max_length = max_length
 
     @property
     def link(self):
         """Gets the link of this FormFieldTextInput.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -169,34 +169,34 @@
 
         :param node_id: The node_id of this FormFieldTextInput.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def calculate_on_exit(self):
-        """Gets the calculate_on_exit of this FormFieldTextInput.  # noqa: E501
+    def name(self):
+        """Gets the name of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :return: The calculate_on_exit of this FormFieldTextInput.  # noqa: E501
-        :rtype: bool
+        :return: The name of this FormFieldTextInput.  # noqa: E501
+        :rtype: str
         """
-        return self._calculate_on_exit
+        return self._name
 
-    @calculate_on_exit.setter
-    def calculate_on_exit(self, calculate_on_exit):
-        """Sets the calculate_on_exit of this FormFieldTextInput.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this FormFieldTextInput.
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :param calculate_on_exit: The calculate_on_exit of this FormFieldTextInput.  # noqa: E501
-        :type: bool
+        :param name: The name of this FormFieldTextInput.  # noqa: E501
+        :type: str
         """
-        self._calculate_on_exit = calculate_on_exit
+        self._name = name
 
     @property
     def enabled(self):
         """Gets the enabled of this FormFieldTextInput.  # noqa: E501
 
         Gets or sets a value indicating whether a form field is enabled.  # noqa: E501
 
@@ -213,56 +213,56 @@
 
         :param enabled: The enabled of this FormFieldTextInput.  # noqa: E501
         :type: bool
         """
         self._enabled = enabled
 
     @property
-    def entry_macro(self):
-        """Gets the entry_macro of this FormFieldTextInput.  # noqa: E501
+    def status_text(self):
+        """Gets the status_text of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The entry_macro of this FormFieldTextInput.  # noqa: E501
+        :return: The status_text of this FormFieldTextInput.  # noqa: E501
         :rtype: str
         """
-        return self._entry_macro
+        return self._status_text
 
-    @entry_macro.setter
-    def entry_macro(self, entry_macro):
-        """Sets the entry_macro of this FormFieldTextInput.
+    @status_text.setter
+    def status_text(self, status_text):
+        """Sets the status_text of this FormFieldTextInput.
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param entry_macro: The entry_macro of this FormFieldTextInput.  # noqa: E501
+        :param status_text: The status_text of this FormFieldTextInput.  # noqa: E501
         :type: str
         """
-        self._entry_macro = entry_macro
+        self._status_text = status_text
 
     @property
-    def exit_macro(self):
-        """Gets the exit_macro of this FormFieldTextInput.  # noqa: E501
+    def own_status(self):
+        """Gets the own_status of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The exit_macro of this FormFieldTextInput.  # noqa: E501
-        :rtype: str
+        :return: The own_status of this FormFieldTextInput.  # noqa: E501
+        :rtype: bool
         """
-        return self._exit_macro
+        return self._own_status
 
-    @exit_macro.setter
-    def exit_macro(self, exit_macro):
-        """Sets the exit_macro of this FormFieldTextInput.
+    @own_status.setter
+    def own_status(self, own_status):
+        """Sets the own_status of this FormFieldTextInput.
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param exit_macro: The exit_macro of this FormFieldTextInput.  # noqa: E501
-        :type: str
+        :param own_status: The own_status of this FormFieldTextInput.  # noqa: E501
+        :type: bool
         """
-        self._exit_macro = exit_macro
+        self._own_status = own_status
 
     @property
     def help_text(self):
         """Gets the help_text of this FormFieldTextInput.  # noqa: E501
 
         Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1.  # noqa: E501
 
@@ -279,36 +279,14 @@
 
         :param help_text: The help_text of this FormFieldTextInput.  # noqa: E501
         :type: str
         """
         self._help_text = help_text
 
     @property
-    def name(self):
-        """Gets the name of this FormFieldTextInput.  # noqa: E501
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :return: The name of this FormFieldTextInput.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this FormFieldTextInput.
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :param name: The name of this FormFieldTextInput.  # noqa: E501
-        :type: str
-        """
-        self._name = name
-
-    @property
     def own_help(self):
         """Gets the own_help of this FormFieldTextInput.  # noqa: E501
 
         Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1.  # noqa: E501
 
         :return: The own_help of this FormFieldTextInput.  # noqa: E501
         :rtype: bool
@@ -323,100 +301,78 @@
 
         :param own_help: The own_help of this FormFieldTextInput.  # noqa: E501
         :type: bool
         """
         self._own_help = own_help
 
     @property
-    def own_status(self):
-        """Gets the own_status of this FormFieldTextInput.  # noqa: E501
+    def calculate_on_exit(self):
+        """Gets the calculate_on_exit of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :return: The own_status of this FormFieldTextInput.  # noqa: E501
+        :return: The calculate_on_exit of this FormFieldTextInput.  # noqa: E501
         :rtype: bool
         """
-        return self._own_status
+        return self._calculate_on_exit
 
-    @own_status.setter
-    def own_status(self, own_status):
-        """Sets the own_status of this FormFieldTextInput.
+    @calculate_on_exit.setter
+    def calculate_on_exit(self, calculate_on_exit):
+        """Sets the calculate_on_exit of this FormFieldTextInput.
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :param own_status: The own_status of this FormFieldTextInput.  # noqa: E501
+        :param calculate_on_exit: The calculate_on_exit of this FormFieldTextInput.  # noqa: E501
         :type: bool
         """
-        self._own_status = own_status
+        self._calculate_on_exit = calculate_on_exit
 
     @property
-    def status_text(self):
-        """Gets the status_text of this FormFieldTextInput.  # noqa: E501
+    def entry_macro(self):
+        """Gets the entry_macro of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :return: The status_text of this FormFieldTextInput.  # noqa: E501
+        :return: The entry_macro of this FormFieldTextInput.  # noqa: E501
         :rtype: str
         """
-        return self._status_text
+        return self._entry_macro
 
-    @status_text.setter
-    def status_text(self, status_text):
-        """Sets the status_text of this FormFieldTextInput.
+    @entry_macro.setter
+    def entry_macro(self, entry_macro):
+        """Sets the entry_macro of this FormFieldTextInput.
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :param status_text: The status_text of this FormFieldTextInput.  # noqa: E501
+        :param entry_macro: The entry_macro of this FormFieldTextInput.  # noqa: E501
         :type: str
         """
-        self._status_text = status_text
-
-    @property
-    def max_length(self):
-        """Gets the max_length of this FormFieldTextInput.  # noqa: E501
-
-        Gets or sets the maximum length for the text field. Zero when the length is not limited.  # noqa: E501
-
-        :return: The max_length of this FormFieldTextInput.  # noqa: E501
-        :rtype: int
-        """
-        return self._max_length
-
-    @max_length.setter
-    def max_length(self, max_length):
-        """Sets the max_length of this FormFieldTextInput.
-
-        Gets or sets the maximum length for the text field. Zero when the length is not limited.  # noqa: E501
-
-        :param max_length: The max_length of this FormFieldTextInput.  # noqa: E501
-        :type: int
-        """
-        self._max_length = max_length
+        self._entry_macro = entry_macro
 
     @property
-    def text_input_default(self):
-        """Gets the text_input_default of this FormFieldTextInput.  # noqa: E501
+    def exit_macro(self):
+        """Gets the exit_macro of this FormFieldTextInput.  # noqa: E501
 
-        Gets or sets the default string or a calculation expression of the text form field.  # noqa: E501
+        Gets or sets the exit macro name for the form field.  # noqa: E501
 
-        :return: The text_input_default of this FormFieldTextInput.  # noqa: E501
+        :return: The exit_macro of this FormFieldTextInput.  # noqa: E501
         :rtype: str
         """
-        return self._text_input_default
+        return self._exit_macro
 
-    @text_input_default.setter
-    def text_input_default(self, text_input_default):
-        """Sets the text_input_default of this FormFieldTextInput.
+    @exit_macro.setter
+    def exit_macro(self, exit_macro):
+        """Sets the exit_macro of this FormFieldTextInput.
 
-        Gets or sets the default string or a calculation expression of the text form field.  # noqa: E501
+        Gets or sets the exit macro name for the form field.  # noqa: E501
 
-        :param text_input_default: The text_input_default of this FormFieldTextInput.  # noqa: E501
+        :param exit_macro: The exit_macro of this FormFieldTextInput.  # noqa: E501
         :type: str
         """
-        self._text_input_default = text_input_default
+        self._exit_macro = exit_macro
 
     @property
     def text_input_format(self):
         """Gets the text_input_format of this FormFieldTextInput.  # noqa: E501
 
         Gets or sets text formatting for the text form field.  # noqa: E501
 
@@ -462,14 +418,58 @@
                 raise ValueError(
                     "Invalid value for `text_input_type` ({0}), must be one of {1}"  # noqa: E501
                     .format(text_input_type, allowed_values))
             self._text_input_type = text_input_type
         else:
             self._text_input_type = allowed_values[int(text_input_type) if six.PY3 else long(text_input_type)]
 
+    @property
+    def text_input_default(self):
+        """Gets the text_input_default of this FormFieldTextInput.  # noqa: E501
+
+        Gets or sets the default string or a calculation expression of the text form field.  # noqa: E501
+
+        :return: The text_input_default of this FormFieldTextInput.  # noqa: E501
+        :rtype: str
+        """
+        return self._text_input_default
+
+    @text_input_default.setter
+    def text_input_default(self, text_input_default):
+        """Sets the text_input_default of this FormFieldTextInput.
+
+        Gets or sets the default string or a calculation expression of the text form field.  # noqa: E501
+
+        :param text_input_default: The text_input_default of this FormFieldTextInput.  # noqa: E501
+        :type: str
+        """
+        self._text_input_default = text_input_default
+
+    @property
+    def max_length(self):
+        """Gets the max_length of this FormFieldTextInput.  # noqa: E501
+
+        Gets or sets the maximum length for the text field. Zero when the length is not limited.  # noqa: E501
+
+        :return: The max_length of this FormFieldTextInput.  # noqa: E501
+        :rtype: int
+        """
+        return self._max_length
+
+    @max_length.setter
+    def max_length(self, max_length):
+        """Sets the max_length of this FormFieldTextInput.
+
+        Gets or sets the maximum length for the text field. Zero when the length is not limited.  # noqa: E501
+
+        :param max_length: The max_length of this FormFieldTextInput.  # noqa: E501
+        :type: int
+        """
+        self._max_length = max_length
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/font_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/font_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/user_information.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/user_information.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/replace_text_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,50 +40,50 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'child_nodes': 'list[NodeLink]',
-        'header_footers': 'LinkElement',
-        'page_setup': 'LinkElement',
         'paragraphs': 'LinkElement',
+        'page_setup': 'LinkElement',
+        'header_footers': 'LinkElement',
         'tables': 'LinkElement'
     }
 
     attribute_map = {
         'link': 'Link',
         'child_nodes': 'ChildNodes',
-        'header_footers': 'HeaderFooters',
-        'page_setup': 'PageSetup',
         'paragraphs': 'Paragraphs',
+        'page_setup': 'PageSetup',
+        'header_footers': 'HeaderFooters',
         'tables': 'Tables'
     }
 
-    def __init__(self, link=None, child_nodes=None, header_footers=None, page_setup=None, paragraphs=None, tables=None):  # noqa: E501
+    def __init__(self, link=None, child_nodes=None, paragraphs=None, page_setup=None, header_footers=None, tables=None):  # noqa: E501
         """Section - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._child_nodes = None
-        self._header_footers = None
-        self._page_setup = None
         self._paragraphs = None
+        self._page_setup = None
+        self._header_footers = None
         self._tables = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if child_nodes is not None:
             self.child_nodes = child_nodes
-        if header_footers is not None:
-            self.header_footers = header_footers
-        if page_setup is not None:
-            self.page_setup = page_setup
         if paragraphs is not None:
             self.paragraphs = paragraphs
+        if page_setup is not None:
+            self.page_setup = page_setup
+        if header_footers is not None:
+            self.header_footers = header_footers
         if tables is not None:
             self.tables = tables
 
     @property
     def link(self):
         """Gets the link of this Section.  # noqa: E501
 
@@ -124,34 +124,34 @@
 
         :param child_nodes: The child_nodes of this Section.  # noqa: E501
         :type: list[NodeLink]
         """
         self._child_nodes = child_nodes
 
     @property
-    def header_footers(self):
-        """Gets the header_footers of this Section.  # noqa: E501
+    def paragraphs(self):
+        """Gets the paragraphs of this Section.  # noqa: E501
 
-        Gets or sets the link to HeaderFooters resource.  # noqa: E501
+        Gets or sets the link to Paragraphs resource.  # noqa: E501
 
-        :return: The header_footers of this Section.  # noqa: E501
+        :return: The paragraphs of this Section.  # noqa: E501
         :rtype: LinkElement
         """
-        return self._header_footers
+        return self._paragraphs
 
-    @header_footers.setter
-    def header_footers(self, header_footers):
-        """Sets the header_footers of this Section.
+    @paragraphs.setter
+    def paragraphs(self, paragraphs):
+        """Sets the paragraphs of this Section.
 
-        Gets or sets the link to HeaderFooters resource.  # noqa: E501
+        Gets or sets the link to Paragraphs resource.  # noqa: E501
 
-        :param header_footers: The header_footers of this Section.  # noqa: E501
+        :param paragraphs: The paragraphs of this Section.  # noqa: E501
         :type: LinkElement
         """
-        self._header_footers = header_footers
+        self._paragraphs = paragraphs
 
     @property
     def page_setup(self):
         """Gets the page_setup of this Section.  # noqa: E501
 
         Gets or sets the link to PageSetup resource.  # noqa: E501
 
@@ -168,34 +168,34 @@
 
         :param page_setup: The page_setup of this Section.  # noqa: E501
         :type: LinkElement
         """
         self._page_setup = page_setup
 
     @property
-    def paragraphs(self):
-        """Gets the paragraphs of this Section.  # noqa: E501
+    def header_footers(self):
+        """Gets the header_footers of this Section.  # noqa: E501
 
-        Gets or sets the link to Paragraphs resource.  # noqa: E501
+        Gets or sets the link to HeaderFooters resource.  # noqa: E501
 
-        :return: The paragraphs of this Section.  # noqa: E501
+        :return: The header_footers of this Section.  # noqa: E501
         :rtype: LinkElement
         """
-        return self._paragraphs
+        return self._header_footers
 
-    @paragraphs.setter
-    def paragraphs(self, paragraphs):
-        """Sets the paragraphs of this Section.
+    @header_footers.setter
+    def header_footers(self, header_footers):
+        """Sets the header_footers of this Section.
 
-        Gets or sets the link to Paragraphs resource.  # noqa: E501
+        Gets or sets the link to HeaderFooters resource.  # noqa: E501
 
-        :param paragraphs: The paragraphs of this Section.  # noqa: E501
+        :param header_footers: The header_footers of this Section.  # noqa: E501
         :type: LinkElement
         """
-        self._paragraphs = paragraphs
+        self._header_footers = header_footers
 
     @property
     def tables(self):
         """Gets the tables of this Section.  # noqa: E501
 
         Gets or sets the link to Tables resource.  # noqa: E501
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/__init__.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/runs_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/runs_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_insert_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/run_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/run_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/time_zone_info_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/time_zone_info_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/protection_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/metafile_rendering_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/metafile_rendering_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/replace_text_parameters.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_text_parameters.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/search_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/search_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/search_results_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/search_results_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/drawing_object_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/drawing_object_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_level_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_level_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_property_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/file_reference.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/file_reference.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/tab_stop_base.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/tab_stop_base.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/html_fixed_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/html_fixed_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,17 +70,17 @@
         'export_form_fields': 'bool',
         'font_format': 'str',
         'page_horizontal_alignment': 'str',
         'page_margins': 'float',
         'resources_folder': 'str',
         'resources_folder_alias': 'str',
         'save_font_face_css_separately': 'bool',
-        'save_format': 'str',
         'show_page_border': 'bool',
-        'use_target_machine_fonts': 'bool'
+        'use_target_machine_fonts': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -108,17 +108,17 @@
         'export_form_fields': 'ExportFormFields',
         'font_format': 'FontFormat',
         'page_horizontal_alignment': 'PageHorizontalAlignment',
         'page_margins': 'PageMargins',
         'resources_folder': 'ResourcesFolder',
         'resources_folder_alias': 'ResourcesFolderAlias',
         'save_font_face_css_separately': 'SaveFontFaceCssSeparately',
-        'save_format': 'SaveFormat',
         'show_page_border': 'ShowPageBorder',
-        'use_target_machine_fonts': 'UseTargetMachineFonts'
+        'use_target_machine_fonts': 'UseTargetMachineFonts',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, css_class_names_prefix=None, encoding=None, export_embedded_css=None, export_embedded_fonts=None, export_embedded_images=None, export_form_fields=None, font_format=None, page_horizontal_alignment=None, page_margins=None, resources_folder=None, resources_folder_alias=None, save_font_face_css_separately=None, show_page_border=None, use_target_machine_fonts=None):  # noqa: E501
         """HtmlFixedSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -148,17 +148,17 @@
         self._export_form_fields = None
         self._font_format = None
         self._page_horizontal_alignment = None
         self._page_margins = None
         self._resources_folder = None
         self._resources_folder_alias = None
         self._save_font_face_css_separately = None
-        self._save_format = "htmlfixed"
         self._show_page_border = None
         self._use_target_machine_fonts = None
+        self._save_format = "htmlfixed"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -991,26 +991,14 @@
 
         :param save_font_face_css_separately: The save_font_face_css_separately of this HtmlFixedSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._save_font_face_css_separately = save_font_face_css_separately
 
     @property
-    def save_format(self):
-        """Gets the save_format of this HtmlFixedSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this HtmlFixedSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def show_page_border(self):
         """Gets the show_page_border of this HtmlFixedSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to show border around pages.  # noqa: E501
 
         :return: The show_page_border of this HtmlFixedSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -1046,14 +1034,26 @@
         Gets or sets a value indicating whether fonts from target machine must be used to display the document. If this flag is set to true, Aspose.Words.Saving.HtmlFixedSaveOptions.FontFormat and Aspose.Words.Saving.HtmlFixedSaveOptions.ExportEmbeddedFonts properties do not have effect, also Aspose.Words.Saving.HtmlFixedSaveOptions.ResourceSavingCallback is not fired for fonts. The default value is false.  # noqa: E501
 
         :param use_target_machine_fonts: The use_target_machine_fonts of this HtmlFixedSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_target_machine_fonts = use_target_machine_fonts
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this HtmlFixedSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this HtmlFixedSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/replace_range.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/replace_range.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/runs.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/runs.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/files_upload_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/outline_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/outline_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_position.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_position.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/border.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_list_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_page_numbers_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/append_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraphs_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_folder_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_border_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/build_report_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_properties_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_section_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comments_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmark_by_name_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmarks_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comments_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comments_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_section_page_setup_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/move_file_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_of_section_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comment_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/build_report_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/build_report_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_file_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_objects_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/split_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_range_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_borders_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_cell_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_with_text_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_statistics_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_structured_document_tag_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_from_document_element_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reject_all_revisions_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_cell_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/execute_mail_merge_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_watermark_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_form_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/load_web_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/load_web_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_borders_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlinks_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_or_update_document_property_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_tables_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_runs_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_image_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/protect_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_fields_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_list_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_list_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_footnote_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_style_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_drawing_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_math_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_document_property_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_comment_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_all_paragraph_tab_stops_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraphs_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraphs_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_image_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_image_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_form_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_with_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_with_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_tab_stops_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_part_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_paragraph_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_protection_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_folder_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_lists_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_table_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_structured_document_tag_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_field_names_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_properties_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_header_footer_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_text_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_row_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/unprotect_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_list_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_style_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_lists_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_lists_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_macros_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_cell_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/batch_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/batch_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_part_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmark_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_border_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_drawing_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_table_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_table_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_row_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_row_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_border_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_objects_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_border_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_border_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnote_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_level_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_math_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_tiff_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/optimize_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_row_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_row_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_info_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_info_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_section_page_setup_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_properties_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_office_math_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_page_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compress_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_paragraph_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compress_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compress_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_font_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_fields_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footers_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/move_folder_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_fields_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_properties_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_fields_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_custom_xml_parts_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_objects_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_objects_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_page_setup_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comment_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tag_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/download_file_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_page_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_page_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_bookmark_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_style_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_style_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_run_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_drawing_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_custom_xml_part_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_run_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_footnote_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_bookmark_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_form_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compare_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_form_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tags_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/remove_range_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnotes_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_borders_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_borders_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_list_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_headers_footers_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/append_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/append_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_footnote_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_footnote_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_fields_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/accept_all_revisions_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmarks_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_custom_xml_part_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/__init__.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tag_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_bookmark_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_footnote_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_properties_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_macros_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_macros_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_of_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/search_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_text_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_property_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_property_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmarks_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmarks_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/link_header_footers_to_previous_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/link_header_footers_to_previous_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_style_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_style_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_text_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_style_from_document_element_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_style_from_document_element_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_tiff_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_tiff_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_objects_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_comment_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_page_setup_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_office_math_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/copy_styles_from_template_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/copy_styles_from_template_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_form_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reset_cache_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reset_cache_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_range_text_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_header_footer_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_comment_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/reject_all_revisions_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/reject_all_revisions_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlinks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_section_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/remove_range_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/remove_range_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_structured_document_tags_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_structured_document_tags_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_row_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_part_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_cell_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_cell_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_range_text_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_range_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_section_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_borders_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_borders_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_watermark_text_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_watermark_text_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_protection_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_protection_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_run_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_or_update_document_property_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_or_update_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/apply_style_to_document_element_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/apply_style_to_document_element_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_styles_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_page_numbers_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_page_numbers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_sections_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_header_footer_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnote_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnote_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_bookmark_by_name_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_custom_xml_part_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_custom_xml_part_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_list_level_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_list_level_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footers_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footers_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/create_folder_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_structured_document_tag_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_drawing_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/search_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/search_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_drawing_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_table_cell_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_comment_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_comment_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_watermark_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_watermark_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_statistics_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_statistics_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/optimize_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/optimize_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_drawing_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_parts_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_footnote_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_footnote_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_available_fonts_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_available_fonts_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_drawing_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_drawing_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_run_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_run_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/base_request_object.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/base_request_object.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_border_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_form_field_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_form_field_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_files_list_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_structured_document_tag_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_list_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/split_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/split_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_field_names_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_field_names_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_paragraph_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_bookmark_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_properties_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_properties_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_structured_document_tag_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_structured_document_tag_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/convert_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/convert_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_run_font_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/compare_document_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/compare_document_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_hyperlink_by_index_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_cell_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_cell_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_paragraph_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comment_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_paragraph_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_styles_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_styles_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_section_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_section_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_field_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_field_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_font_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_headers_footers_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_headers_footers_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_style_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_style_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_format_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_format_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/protect_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/protect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_form_fields_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_form_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_table_row_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_table_row_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_table_cell_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_table_cell_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_list_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_list_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmark_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmark_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/execute_mail_merge_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/execute_mail_merge_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_fields_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_fields_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/classify_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/classify_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_runs_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_runs_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_drawing_object_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_drawing_object_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_border_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_border_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_comments_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_comments_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_office_math_object_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_office_math_object_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_bookmarks_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_bookmarks_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_ole_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/save_as_range_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/save_as_range_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_custom_xml_parts_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_document_property_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_document_property_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_comment_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_comment_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/unprotect_document_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/unprotect_document_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_document_drawing_object_image_data_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/render_paragraph_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/render_paragraph_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/upload_file_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_run_font_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_run_font_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/update_paragraph_list_format_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_public_key_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_public_key_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_header_footer_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_fields_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_fields_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_tables_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_tables_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_table_row_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_table_row_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/accept_all_revisions_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/accept_all_revisions_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_file_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_footnotes_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_footnotes_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/get_sections_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/get_sections_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/replace_with_text_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/replace_with_text_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_section_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_section_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/insert_or_update_paragraph_tab_stop_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/requests/delete_header_footer_online_request.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/requests/delete_header_footer_online_request.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/flat_opc_template_macro_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/flat_opc_template_macro_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_properties.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_format_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_format_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_property_create_or_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_property_create_or_update.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_flow_pack_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_pack_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/emf_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/emf_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,17 +67,17 @@
         'image_color_mode': 'str',
         'image_contrast': 'float',
         'paper_color': 'str',
         'pixel_format': 'str',
         'resolution': 'float',
         'scale': 'float',
         'use_anti_aliasing': 'bool',
-        'use_gdi_emf_renderer': 'bool',
         'use_high_quality_rendering': 'bool',
         'vertical_resolution': 'float',
+        'use_gdi_emf_renderer': 'bool',
         'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
@@ -103,21 +103,21 @@
         'image_color_mode': 'ImageColorMode',
         'image_contrast': 'ImageContrast',
         'paper_color': 'PaperColor',
         'pixel_format': 'PixelFormat',
         'resolution': 'Resolution',
         'scale': 'Scale',
         'use_anti_aliasing': 'UseAntiAliasing',
-        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'use_high_quality_rendering': 'UseHighQualityRendering',
         'vertical_resolution': 'VerticalResolution',
+        'use_gdi_emf_renderer': 'UseGdiEmfRenderer',
         'save_format': 'SaveFormat'
     }
 
-    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_gdi_emf_renderer=None, use_high_quality_rendering=None, vertical_resolution=None):  # noqa: E501
+    def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, color_mode=None, jpeg_quality=None, metafile_rendering_options=None, numeral_format=None, optimize_output=None, page_count=None, page_index=None, horizontal_resolution=None, image_brightness=None, image_color_mode=None, image_contrast=None, paper_color=None, pixel_format=None, resolution=None, scale=None, use_anti_aliasing=None, use_high_quality_rendering=None, vertical_resolution=None, use_gdi_emf_renderer=None):  # noqa: E501
         """EmfSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
         self._dml3_d_effects_rendering_mode = None
         self._dml_effects_rendering_mode = None
         self._dml_rendering_mode = None
@@ -141,17 +141,17 @@
         self._image_color_mode = None
         self._image_contrast = None
         self._paper_color = None
         self._pixel_format = None
         self._resolution = None
         self._scale = None
         self._use_anti_aliasing = None
-        self._use_gdi_emf_renderer = None
         self._use_high_quality_rendering = None
         self._vertical_resolution = None
+        self._use_gdi_emf_renderer = None
         self._save_format = "emf"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
@@ -205,20 +205,20 @@
             self.pixel_format = pixel_format
         if resolution is not None:
             self.resolution = resolution
         if scale is not None:
             self.scale = scale
         if use_anti_aliasing is not None:
             self.use_anti_aliasing = use_anti_aliasing
-        if use_gdi_emf_renderer is not None:
-            self.use_gdi_emf_renderer = use_gdi_emf_renderer
         if use_high_quality_rendering is not None:
             self.use_high_quality_rendering = use_high_quality_rendering
         if vertical_resolution is not None:
             self.vertical_resolution = vertical_resolution
+        if use_gdi_emf_renderer is not None:
+            self.use_gdi_emf_renderer = use_gdi_emf_renderer
 
     @property
     def allow_embedding_post_script_fonts(self):
         """Gets the allow_embedding_post_script_fonts of this EmfSaveOptionsData.  # noqa: E501
 
         Gets or sets a boolean value indicating whether to allow embedding fonts with PostScript outlines when embedding TrueType fonts in a document upon it is saved. The default value is false..  # noqa: E501
 
@@ -915,36 +915,14 @@
 
         :param use_anti_aliasing: The use_anti_aliasing of this EmfSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._use_anti_aliasing = use_anti_aliasing
 
     @property
-    def use_gdi_emf_renderer(self):
-        """Gets the use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :return: The use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
-        :rtype: bool
-        """
-        return self._use_gdi_emf_renderer
-
-    @use_gdi_emf_renderer.setter
-    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
-        """Sets the use_gdi_emf_renderer of this EmfSaveOptionsData.
-
-        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
-
-        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
-        :type: bool
-        """
-        self._use_gdi_emf_renderer = use_gdi_emf_renderer
-
-    @property
     def use_high_quality_rendering(self):
         """Gets the use_high_quality_rendering of this EmfSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether to use high quality (i.e. slow) rendering algorithms.  # noqa: E501
 
         :return: The use_high_quality_rendering of this EmfSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -981,14 +959,36 @@
 
         :param vertical_resolution: The vertical_resolution of this EmfSaveOptionsData.  # noqa: E501
         :type: float
         """
         self._vertical_resolution = vertical_resolution
 
     @property
+    def use_gdi_emf_renderer(self):
+        """Gets the use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :return: The use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
+        :rtype: bool
+        """
+        return self._use_gdi_emf_renderer
+
+    @use_gdi_emf_renderer.setter
+    def use_gdi_emf_renderer(self, use_gdi_emf_renderer):
+        """Sets the use_gdi_emf_renderer of this EmfSaveOptionsData.
+
+        Gets or sets a value indicating whether to use GDI+ or Aspose.Words metafile renderer when saving to EMF.  # noqa: E501
+
+        :param use_gdi_emf_renderer: The use_gdi_emf_renderer of this EmfSaveOptionsData.  # noqa: E501
+        :type: bool
+        """
+        self._use_gdi_emf_renderer = use_gdi_emf_renderer
+
+    @property
     def save_format(self):
         """Gets the save_format of this EmfSaveOptionsData.  # noqa: E501
 
         Gets the format of save.  # noqa: E501
 
         :return: The save_format of this EmfSaveOptionsData.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_base.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,24 +55,24 @@
         'line_spacing': 'float',
         'line_spacing_rule': 'str',
         'lines_to_drop': 'int',
         'no_space_between_paragraphs_of_same_style': 'bool',
         'outline_level': 'str',
         'page_break_before': 'bool',
         'right_indent': 'float',
-        'shading': 'Shading',
         'space_after': 'float',
         'space_after_auto': 'bool',
         'space_before': 'float',
         'space_before_auto': 'bool',
         'style_identifier': 'str',
         'style_name': 'str',
         'suppress_auto_hyphens': 'bool',
         'suppress_line_numbers': 'bool',
-        'widow_control': 'bool'
+        'widow_control': 'bool',
+        'shading': 'Shading'
     }
 
     attribute_map = {
         'link': 'Link',
         'add_space_between_far_east_and_alpha': 'AddSpaceBetweenFarEastAndAlpha',
         'add_space_between_far_east_and_digit': 'AddSpaceBetweenFarEastAndDigit',
         'alignment': 'Alignment',
@@ -85,27 +85,27 @@
         'line_spacing': 'LineSpacing',
         'line_spacing_rule': 'LineSpacingRule',
         'lines_to_drop': 'LinesToDrop',
         'no_space_between_paragraphs_of_same_style': 'NoSpaceBetweenParagraphsOfSameStyle',
         'outline_level': 'OutlineLevel',
         'page_break_before': 'PageBreakBefore',
         'right_indent': 'RightIndent',
-        'shading': 'Shading',
         'space_after': 'SpaceAfter',
         'space_after_auto': 'SpaceAfterAuto',
         'space_before': 'SpaceBefore',
         'space_before_auto': 'SpaceBeforeAuto',
         'style_identifier': 'StyleIdentifier',
         'style_name': 'StyleName',
         'suppress_auto_hyphens': 'SuppressAutoHyphens',
         'suppress_line_numbers': 'SuppressLineNumbers',
-        'widow_control': 'WidowControl'
+        'widow_control': 'WidowControl',
+        'shading': 'Shading'
     }
 
-    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, shading=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None):  # noqa: E501
+    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None, shading=None):  # noqa: E501
         """ParagraphFormatBase - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._add_space_between_far_east_and_alpha = None
         self._add_space_between_far_east_and_digit = None
         self._alignment = None
         self._bidi = None
@@ -117,24 +117,24 @@
         self._line_spacing = None
         self._line_spacing_rule = None
         self._lines_to_drop = None
         self._no_space_between_paragraphs_of_same_style = None
         self._outline_level = None
         self._page_break_before = None
         self._right_indent = None
-        self._shading = None
         self._space_after = None
         self._space_after_auto = None
         self._space_before = None
         self._space_before_auto = None
         self._style_identifier = None
         self._style_name = None
         self._suppress_auto_hyphens = None
         self._suppress_line_numbers = None
         self._widow_control = None
+        self._shading = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if add_space_between_far_east_and_alpha is not None:
             self.add_space_between_far_east_and_alpha = add_space_between_far_east_and_alpha
         if add_space_between_far_east_and_digit is not None:
@@ -163,16 +163,14 @@
             self.no_space_between_paragraphs_of_same_style = no_space_between_paragraphs_of_same_style
         if outline_level is not None:
             self.outline_level = outline_level
         if page_break_before is not None:
             self.page_break_before = page_break_before
         if right_indent is not None:
             self.right_indent = right_indent
-        if shading is not None:
-            self.shading = shading
         if space_after is not None:
             self.space_after = space_after
         if space_after_auto is not None:
             self.space_after_auto = space_after_auto
         if space_before is not None:
             self.space_before = space_before
         if space_before_auto is not None:
@@ -183,14 +181,16 @@
             self.style_name = style_name
         if suppress_auto_hyphens is not None:
             self.suppress_auto_hyphens = suppress_auto_hyphens
         if suppress_line_numbers is not None:
             self.suppress_line_numbers = suppress_line_numbers
         if widow_control is not None:
             self.widow_control = widow_control
+        if shading is not None:
+            self.shading = shading
 
     @property
     def link(self):
         """Gets the link of this ParagraphFormatBase.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -591,36 +591,14 @@
 
         :param right_indent: The right_indent of this ParagraphFormatBase.  # noqa: E501
         :type: float
         """
         self._right_indent = right_indent
 
     @property
-    def shading(self):
-        """Gets the shading of this ParagraphFormatBase.  # noqa: E501
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :return: The shading of this ParagraphFormatBase.  # noqa: E501
-        :rtype: Shading
-        """
-        return self._shading
-
-    @shading.setter
-    def shading(self, shading):
-        """Sets the shading of this ParagraphFormatBase.
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :param shading: The shading of this ParagraphFormatBase.  # noqa: E501
-        :type: Shading
-        """
-        self._shading = shading
-
-    @property
     def space_after(self):
         """Gets the space_after of this ParagraphFormatBase.  # noqa: E501
 
         Gets or sets the amount of spacing (in points) after the paragraph.  # noqa: E501
 
         :return: The space_after of this ParagraphFormatBase.  # noqa: E501
         :rtype: float
@@ -818,14 +796,36 @@
         Gets or sets a value indicating whether the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph.  # noqa: E501
 
         :param widow_control: The widow_control of this ParagraphFormatBase.  # noqa: E501
         :type: bool
         """
         self._widow_control = widow_control
 
+    @property
+    def shading(self):
+        """Gets the shading of this ParagraphFormatBase.  # noqa: E501
+
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
+
+        :return: The shading of this ParagraphFormatBase.  # noqa: E501
+        :rtype: Shading
+        """
+        return self._shading
+
+    @shading.setter
+    def shading(self, shading):
+        """Sets the shading of this ParagraphFormatBase.
+
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
+
+        :param shading: The shading of this ParagraphFormatBase.  # noqa: E501
+        :type: Shading
+        """
+        self._shading = shading
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/shading.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/shading.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/words_api_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/words_api_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,24 +55,24 @@
         'line_spacing': 'float',
         'line_spacing_rule': 'str',
         'lines_to_drop': 'int',
         'no_space_between_paragraphs_of_same_style': 'bool',
         'outline_level': 'str',
         'page_break_before': 'bool',
         'right_indent': 'float',
-        'shading': 'Shading',
         'space_after': 'float',
         'space_after_auto': 'bool',
         'space_before': 'float',
         'space_before_auto': 'bool',
         'style_identifier': 'str',
         'style_name': 'str',
         'suppress_auto_hyphens': 'bool',
         'suppress_line_numbers': 'bool',
-        'widow_control': 'bool'
+        'widow_control': 'bool',
+        'shading': 'Shading'
     }
 
     attribute_map = {
         'link': 'Link',
         'add_space_between_far_east_and_alpha': 'AddSpaceBetweenFarEastAndAlpha',
         'add_space_between_far_east_and_digit': 'AddSpaceBetweenFarEastAndDigit',
         'alignment': 'Alignment',
@@ -85,27 +85,27 @@
         'line_spacing': 'LineSpacing',
         'line_spacing_rule': 'LineSpacingRule',
         'lines_to_drop': 'LinesToDrop',
         'no_space_between_paragraphs_of_same_style': 'NoSpaceBetweenParagraphsOfSameStyle',
         'outline_level': 'OutlineLevel',
         'page_break_before': 'PageBreakBefore',
         'right_indent': 'RightIndent',
-        'shading': 'Shading',
         'space_after': 'SpaceAfter',
         'space_after_auto': 'SpaceAfterAuto',
         'space_before': 'SpaceBefore',
         'space_before_auto': 'SpaceBeforeAuto',
         'style_identifier': 'StyleIdentifier',
         'style_name': 'StyleName',
         'suppress_auto_hyphens': 'SuppressAutoHyphens',
         'suppress_line_numbers': 'SuppressLineNumbers',
-        'widow_control': 'WidowControl'
+        'widow_control': 'WidowControl',
+        'shading': 'Shading'
     }
 
-    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, shading=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None):  # noqa: E501
+    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None, shading=None):  # noqa: E501
         """ParagraphFormatUpdate - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._add_space_between_far_east_and_alpha = None
         self._add_space_between_far_east_and_digit = None
         self._alignment = None
         self._bidi = None
@@ -117,24 +117,24 @@
         self._line_spacing = None
         self._line_spacing_rule = None
         self._lines_to_drop = None
         self._no_space_between_paragraphs_of_same_style = None
         self._outline_level = None
         self._page_break_before = None
         self._right_indent = None
-        self._shading = None
         self._space_after = None
         self._space_after_auto = None
         self._space_before = None
         self._space_before_auto = None
         self._style_identifier = None
         self._style_name = None
         self._suppress_auto_hyphens = None
         self._suppress_line_numbers = None
         self._widow_control = None
+        self._shading = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if add_space_between_far_east_and_alpha is not None:
             self.add_space_between_far_east_and_alpha = add_space_between_far_east_and_alpha
         if add_space_between_far_east_and_digit is not None:
@@ -163,16 +163,14 @@
             self.no_space_between_paragraphs_of_same_style = no_space_between_paragraphs_of_same_style
         if outline_level is not None:
             self.outline_level = outline_level
         if page_break_before is not None:
             self.page_break_before = page_break_before
         if right_indent is not None:
             self.right_indent = right_indent
-        if shading is not None:
-            self.shading = shading
         if space_after is not None:
             self.space_after = space_after
         if space_after_auto is not None:
             self.space_after_auto = space_after_auto
         if space_before is not None:
             self.space_before = space_before
         if space_before_auto is not None:
@@ -183,14 +181,16 @@
             self.style_name = style_name
         if suppress_auto_hyphens is not None:
             self.suppress_auto_hyphens = suppress_auto_hyphens
         if suppress_line_numbers is not None:
             self.suppress_line_numbers = suppress_line_numbers
         if widow_control is not None:
             self.widow_control = widow_control
+        if shading is not None:
+            self.shading = shading
 
     @property
     def link(self):
         """Gets the link of this ParagraphFormatUpdate.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -591,36 +591,14 @@
 
         :param right_indent: The right_indent of this ParagraphFormatUpdate.  # noqa: E501
         :type: float
         """
         self._right_indent = right_indent
 
     @property
-    def shading(self):
-        """Gets the shading of this ParagraphFormatUpdate.  # noqa: E501
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :return: The shading of this ParagraphFormatUpdate.  # noqa: E501
-        :rtype: Shading
-        """
-        return self._shading
-
-    @shading.setter
-    def shading(self, shading):
-        """Sets the shading of this ParagraphFormatUpdate.
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :param shading: The shading of this ParagraphFormatUpdate.  # noqa: E501
-        :type: Shading
-        """
-        self._shading = shading
-
-    @property
     def space_after(self):
         """Gets the space_after of this ParagraphFormatUpdate.  # noqa: E501
 
         Gets or sets the amount of spacing (in points) after the paragraph.  # noqa: E501
 
         :return: The space_after of this ParagraphFormatUpdate.  # noqa: E501
         :rtype: float
@@ -818,14 +796,36 @@
         Gets or sets a value indicating whether the first and last lines in the paragraph are to remain on the same page as the rest of the paragraph.  # noqa: E501
 
         :param widow_control: The widow_control of this ParagraphFormatUpdate.  # noqa: E501
         :type: bool
         """
         self._widow_control = widow_control
 
+    @property
+    def shading(self):
+        """Gets the shading of this ParagraphFormatUpdate.  # noqa: E501
+
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
+
+        :return: The shading of this ParagraphFormatUpdate.  # noqa: E501
+        :rtype: Shading
+        """
+        return self._shading
+
+    @shading.setter
+    def shading(self, shading):
+        """Sets the shading of this ParagraphFormatUpdate.
+
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
+
+        :param shading: The shading of this ParagraphFormatUpdate.  # noqa: E501
+        :type: Shading
+        """
+        self._shading = shading
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/public_key_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/public_key_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/error.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmark_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmark_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_names_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_names_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/docx_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/docx_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comment_update.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,56 +38,100 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'range_start': 'NewDocumentPosition',
+        'range_end': 'NewDocumentPosition',
         'author': 'str',
         'date_time': 'datetime',
         'initial': 'str',
-        'range_end': 'NewDocumentPosition',
-        'range_start': 'NewDocumentPosition',
         'text': 'str'
     }
 
     attribute_map = {
+        'range_start': 'RangeStart',
+        'range_end': 'RangeEnd',
         'author': 'Author',
         'date_time': 'DateTime',
         'initial': 'Initial',
-        'range_end': 'RangeEnd',
-        'range_start': 'RangeStart',
         'text': 'Text'
     }
 
-    def __init__(self, author=None, date_time=None, initial=None, range_end=None, range_start=None, text=None):  # noqa: E501
+    def __init__(self, range_start=None, range_end=None, author=None, date_time=None, initial=None, text=None):  # noqa: E501
         """CommentUpdate - a model defined in Swagger"""  # noqa: E501
 
+        self._range_start = None
+        self._range_end = None
         self._author = None
         self._date_time = None
         self._initial = None
-        self._range_end = None
-        self._range_start = None
         self._text = None
         self.discriminator = None
 
+        if range_start is not None:
+            self.range_start = range_start
+        if range_end is not None:
+            self.range_end = range_end
         if author is not None:
             self.author = author
         if date_time is not None:
             self.date_time = date_time
         if initial is not None:
             self.initial = initial
-        if range_end is not None:
-            self.range_end = range_end
-        if range_start is not None:
-            self.range_start = range_start
         if text is not None:
             self.text = text
 
     @property
+    def range_start(self):
+        """Gets the range_start of this CommentUpdate.  # noqa: E501
+
+        Gets or sets the link to comment range start node.  # noqa: E501
+
+        :return: The range_start of this CommentUpdate.  # noqa: E501
+        :rtype: NewDocumentPosition
+        """
+        return self._range_start
+
+    @range_start.setter
+    def range_start(self, range_start):
+        """Sets the range_start of this CommentUpdate.
+
+        Gets or sets the link to comment range start node.  # noqa: E501
+
+        :param range_start: The range_start of this CommentUpdate.  # noqa: E501
+        :type: NewDocumentPosition
+        """
+        self._range_start = range_start
+
+    @property
+    def range_end(self):
+        """Gets the range_end of this CommentUpdate.  # noqa: E501
+
+        Gets or sets the link to comment range end node.  # noqa: E501
+
+        :return: The range_end of this CommentUpdate.  # noqa: E501
+        :rtype: NewDocumentPosition
+        """
+        return self._range_end
+
+    @range_end.setter
+    def range_end(self, range_end):
+        """Sets the range_end of this CommentUpdate.
+
+        Gets or sets the link to comment range end node.  # noqa: E501
+
+        :param range_end: The range_end of this CommentUpdate.  # noqa: E501
+        :type: NewDocumentPosition
+        """
+        self._range_end = range_end
+
+    @property
     def author(self):
         """Gets the author of this CommentUpdate.  # noqa: E501
 
         Gets or sets the author name for a comment.  # noqa: E501
 
         :return: The author of this CommentUpdate.  # noqa: E501
         :rtype: str
@@ -146,58 +190,14 @@
 
         :param initial: The initial of this CommentUpdate.  # noqa: E501
         :type: str
         """
         self._initial = initial
 
     @property
-    def range_end(self):
-        """Gets the range_end of this CommentUpdate.  # noqa: E501
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :return: The range_end of this CommentUpdate.  # noqa: E501
-        :rtype: NewDocumentPosition
-        """
-        return self._range_end
-
-    @range_end.setter
-    def range_end(self, range_end):
-        """Sets the range_end of this CommentUpdate.
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :param range_end: The range_end of this CommentUpdate.  # noqa: E501
-        :type: NewDocumentPosition
-        """
-        self._range_end = range_end
-
-    @property
-    def range_start(self):
-        """Gets the range_start of this CommentUpdate.  # noqa: E501
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :return: The range_start of this CommentUpdate.  # noqa: E501
-        :rtype: NewDocumentPosition
-        """
-        return self._range_start
-
-    @range_start.setter
-    def range_start(self, range_start):
-        """Sets the range_start of this CommentUpdate.
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :param range_start: The range_start of this CommentUpdate.  # noqa: E501
-        :type: NewDocumentPosition
-        """
-        self._range_start = range_start
-
-    @property
     def text(self):
         """Gets the text of this CommentUpdate.  # noqa: E501
 
         Gets or sets text of the comment.  # noqa: E501
 
         :return: The text of this CommentUpdate.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/stat_data_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/stat_data_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/run_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/run_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_fields_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_fields_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/paragraph_format.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/paragraph_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,26 +55,26 @@
         'line_spacing': 'float',
         'line_spacing_rule': 'str',
         'lines_to_drop': 'int',
         'no_space_between_paragraphs_of_same_style': 'bool',
         'outline_level': 'str',
         'page_break_before': 'bool',
         'right_indent': 'float',
-        'shading': 'Shading',
         'space_after': 'float',
         'space_after_auto': 'bool',
         'space_before': 'float',
         'space_before_auto': 'bool',
         'style_identifier': 'str',
         'style_name': 'str',
         'suppress_auto_hyphens': 'bool',
         'suppress_line_numbers': 'bool',
         'widow_control': 'bool',
-        'is_heading': 'bool',
-        'is_list_item': 'bool'
+        'shading': 'Shading',
+        'is_list_item': 'bool',
+        'is_heading': 'bool'
     }
 
     attribute_map = {
         'link': 'Link',
         'add_space_between_far_east_and_alpha': 'AddSpaceBetweenFarEastAndAlpha',
         'add_space_between_far_east_and_digit': 'AddSpaceBetweenFarEastAndDigit',
         'alignment': 'Alignment',
@@ -87,29 +87,29 @@
         'line_spacing': 'LineSpacing',
         'line_spacing_rule': 'LineSpacingRule',
         'lines_to_drop': 'LinesToDrop',
         'no_space_between_paragraphs_of_same_style': 'NoSpaceBetweenParagraphsOfSameStyle',
         'outline_level': 'OutlineLevel',
         'page_break_before': 'PageBreakBefore',
         'right_indent': 'RightIndent',
-        'shading': 'Shading',
         'space_after': 'SpaceAfter',
         'space_after_auto': 'SpaceAfterAuto',
         'space_before': 'SpaceBefore',
         'space_before_auto': 'SpaceBeforeAuto',
         'style_identifier': 'StyleIdentifier',
         'style_name': 'StyleName',
         'suppress_auto_hyphens': 'SuppressAutoHyphens',
         'suppress_line_numbers': 'SuppressLineNumbers',
         'widow_control': 'WidowControl',
-        'is_heading': 'IsHeading',
-        'is_list_item': 'IsListItem'
+        'shading': 'Shading',
+        'is_list_item': 'IsListItem',
+        'is_heading': 'IsHeading'
     }
 
-    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, shading=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None, is_heading=None, is_list_item=None):  # noqa: E501
+    def __init__(self, link=None, add_space_between_far_east_and_alpha=None, add_space_between_far_east_and_digit=None, alignment=None, bidi=None, drop_cap_position=None, first_line_indent=None, keep_together=None, keep_with_next=None, left_indent=None, line_spacing=None, line_spacing_rule=None, lines_to_drop=None, no_space_between_paragraphs_of_same_style=None, outline_level=None, page_break_before=None, right_indent=None, space_after=None, space_after_auto=None, space_before=None, space_before_auto=None, style_identifier=None, style_name=None, suppress_auto_hyphens=None, suppress_line_numbers=None, widow_control=None, shading=None, is_list_item=None, is_heading=None):  # noqa: E501
         """ParagraphFormat - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._add_space_between_far_east_and_alpha = None
         self._add_space_between_far_east_and_digit = None
         self._alignment = None
         self._bidi = None
@@ -121,26 +121,26 @@
         self._line_spacing = None
         self._line_spacing_rule = None
         self._lines_to_drop = None
         self._no_space_between_paragraphs_of_same_style = None
         self._outline_level = None
         self._page_break_before = None
         self._right_indent = None
-        self._shading = None
         self._space_after = None
         self._space_after_auto = None
         self._space_before = None
         self._space_before_auto = None
         self._style_identifier = None
         self._style_name = None
         self._suppress_auto_hyphens = None
         self._suppress_line_numbers = None
         self._widow_control = None
-        self._is_heading = None
+        self._shading = None
         self._is_list_item = None
+        self._is_heading = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if add_space_between_far_east_and_alpha is not None:
             self.add_space_between_far_east_and_alpha = add_space_between_far_east_and_alpha
         if add_space_between_far_east_and_digit is not None:
@@ -169,16 +169,14 @@
             self.no_space_between_paragraphs_of_same_style = no_space_between_paragraphs_of_same_style
         if outline_level is not None:
             self.outline_level = outline_level
         if page_break_before is not None:
             self.page_break_before = page_break_before
         if right_indent is not None:
             self.right_indent = right_indent
-        if shading is not None:
-            self.shading = shading
         if space_after is not None:
             self.space_after = space_after
         if space_after_auto is not None:
             self.space_after_auto = space_after_auto
         if space_before is not None:
             self.space_before = space_before
         if space_before_auto is not None:
@@ -189,18 +187,20 @@
             self.style_name = style_name
         if suppress_auto_hyphens is not None:
             self.suppress_auto_hyphens = suppress_auto_hyphens
         if suppress_line_numbers is not None:
             self.suppress_line_numbers = suppress_line_numbers
         if widow_control is not None:
             self.widow_control = widow_control
-        if is_heading is not None:
-            self.is_heading = is_heading
+        if shading is not None:
+            self.shading = shading
         if is_list_item is not None:
             self.is_list_item = is_list_item
+        if is_heading is not None:
+            self.is_heading = is_heading
 
     @property
     def link(self):
         """Gets the link of this ParagraphFormat.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -601,36 +601,14 @@
 
         :param right_indent: The right_indent of this ParagraphFormat.  # noqa: E501
         :type: float
         """
         self._right_indent = right_indent
 
     @property
-    def shading(self):
-        """Gets the shading of this ParagraphFormat.  # noqa: E501
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :return: The shading of this ParagraphFormat.  # noqa: E501
-        :rtype: Shading
-        """
-        return self._shading
-
-    @shading.setter
-    def shading(self, shading):
-        """Sets the shading of this ParagraphFormat.
-
-        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
-
-        :param shading: The shading of this ParagraphFormat.  # noqa: E501
-        :type: Shading
-        """
-        self._shading = shading
-
-    @property
     def space_after(self):
         """Gets the space_after of this ParagraphFormat.  # noqa: E501
 
         Gets or sets the amount of spacing (in points) after the paragraph.  # noqa: E501
 
         :return: The space_after of this ParagraphFormat.  # noqa: E501
         :rtype: float
@@ -829,34 +807,34 @@
 
         :param widow_control: The widow_control of this ParagraphFormat.  # noqa: E501
         :type: bool
         """
         self._widow_control = widow_control
 
     @property
-    def is_heading(self):
-        """Gets the is_heading of this ParagraphFormat.  # noqa: E501
+    def shading(self):
+        """Gets the shading of this ParagraphFormat.  # noqa: E501
 
-        Gets or sets a value indicating whether the paragraph style is one of the built-in Heading styles.  # noqa: E501
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
 
-        :return: The is_heading of this ParagraphFormat.  # noqa: E501
-        :rtype: bool
+        :return: The shading of this ParagraphFormat.  # noqa: E501
+        :rtype: Shading
         """
-        return self._is_heading
+        return self._shading
 
-    @is_heading.setter
-    def is_heading(self, is_heading):
-        """Sets the is_heading of this ParagraphFormat.
+    @shading.setter
+    def shading(self, shading):
+        """Sets the shading of this ParagraphFormat.
 
-        Gets or sets a value indicating whether the paragraph style is one of the built-in Heading styles.  # noqa: E501
+        Gets or sets the Shading object, that refers to the shading formatting for the paragraph.  # noqa: E501
 
-        :param is_heading: The is_heading of this ParagraphFormat.  # noqa: E501
-        :type: bool
+        :param shading: The shading of this ParagraphFormat.  # noqa: E501
+        :type: Shading
         """
-        self._is_heading = is_heading
+        self._shading = shading
 
     @property
     def is_list_item(self):
         """Gets the is_list_item of this ParagraphFormat.  # noqa: E501
 
         Gets or sets a value indicating whether the paragraph is an item in a bulleted or numbered list.  # noqa: E501
 
@@ -872,14 +850,36 @@
         Gets or sets a value indicating whether the paragraph is an item in a bulleted or numbered list.  # noqa: E501
 
         :param is_list_item: The is_list_item of this ParagraphFormat.  # noqa: E501
         :type: bool
         """
         self._is_list_item = is_list_item
 
+    @property
+    def is_heading(self):
+        """Gets the is_heading of this ParagraphFormat.  # noqa: E501
+
+        Gets or sets a value indicating whether the paragraph style is one of the built-in Heading styles.  # noqa: E501
+
+        :return: The is_heading of this ParagraphFormat.  # noqa: E501
+        :rtype: bool
+        """
+        return self._is_heading
+
+    @is_heading.setter
+    def is_heading(self, is_heading):
+        """Sets the is_heading of this ParagraphFormat.
+
+        Gets or sets a value indicating whether the paragraph style is one of the built-in Heading styles.  # noqa: E501
+
+        :param is_heading: The is_heading of this ParagraphFormat.  # noqa: E501
+        :type: bool
+        """
+        self._is_heading = is_heading
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/bookmarks.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/bookmarks.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/lists.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/lists.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/list_format.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/list_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,43 +39,43 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'is_list_item': 'bool',
+        'list_level_number': 'int',
         'list_id': 'int',
-        'list_level_number': 'int'
+        'is_list_item': 'bool'
     }
 
     attribute_map = {
         'link': 'Link',
-        'is_list_item': 'IsListItem',
+        'list_level_number': 'ListLevelNumber',
         'list_id': 'ListId',
-        'list_level_number': 'ListLevelNumber'
+        'is_list_item': 'IsListItem'
     }
 
-    def __init__(self, link=None, is_list_item=None, list_id=None, list_level_number=None):  # noqa: E501
+    def __init__(self, link=None, list_level_number=None, list_id=None, is_list_item=None):  # noqa: E501
         """ListFormat - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._is_list_item = None
-        self._list_id = None
         self._list_level_number = None
+        self._list_id = None
+        self._is_list_item = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if is_list_item is not None:
-            self.is_list_item = is_list_item
-        if list_id is not None:
-            self.list_id = list_id
         if list_level_number is not None:
             self.list_level_number = list_level_number
+        if list_id is not None:
+            self.list_id = list_id
+        if is_list_item is not None:
+            self.is_list_item = is_list_item
 
     @property
     def link(self):
         """Gets the link of this ListFormat.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -92,34 +92,34 @@
 
         :param link: The link of this ListFormat.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def is_list_item(self):
-        """Gets the is_list_item of this ListFormat.  # noqa: E501
+    def list_level_number(self):
+        """Gets the list_level_number of this ListFormat.  # noqa: E501
 
-        Gets or sets a value indicating whether the paragraph has bulleted or numbered formatting applied to it.  # noqa: E501
+        Gets or sets the list level number (0 to 8) for the paragraph.  # noqa: E501
 
-        :return: The is_list_item of this ListFormat.  # noqa: E501
-        :rtype: bool
+        :return: The list_level_number of this ListFormat.  # noqa: E501
+        :rtype: int
         """
-        return self._is_list_item
+        return self._list_level_number
 
-    @is_list_item.setter
-    def is_list_item(self, is_list_item):
-        """Sets the is_list_item of this ListFormat.
+    @list_level_number.setter
+    def list_level_number(self, list_level_number):
+        """Sets the list_level_number of this ListFormat.
 
-        Gets or sets a value indicating whether the paragraph has bulleted or numbered formatting applied to it.  # noqa: E501
+        Gets or sets the list level number (0 to 8) for the paragraph.  # noqa: E501
 
-        :param is_list_item: The is_list_item of this ListFormat.  # noqa: E501
-        :type: bool
+        :param list_level_number: The list_level_number of this ListFormat.  # noqa: E501
+        :type: int
         """
-        self._is_list_item = is_list_item
+        self._list_level_number = list_level_number
 
     @property
     def list_id(self):
         """Gets the list_id of this ListFormat.  # noqa: E501
 
         Gets or sets the list id of this paragraph.  # noqa: E501
 
@@ -136,34 +136,34 @@
 
         :param list_id: The list_id of this ListFormat.  # noqa: E501
         :type: int
         """
         self._list_id = list_id
 
     @property
-    def list_level_number(self):
-        """Gets the list_level_number of this ListFormat.  # noqa: E501
+    def is_list_item(self):
+        """Gets the is_list_item of this ListFormat.  # noqa: E501
 
-        Gets or sets the list level number (0 to 8) for the paragraph.  # noqa: E501
+        Gets or sets a value indicating whether the paragraph has bulleted or numbered formatting applied to it.  # noqa: E501
 
-        :return: The list_level_number of this ListFormat.  # noqa: E501
-        :rtype: int
+        :return: The is_list_item of this ListFormat.  # noqa: E501
+        :rtype: bool
         """
-        return self._list_level_number
+        return self._is_list_item
 
-    @list_level_number.setter
-    def list_level_number(self, list_level_number):
-        """Sets the list_level_number of this ListFormat.
+    @is_list_item.setter
+    def is_list_item(self, is_list_item):
+        """Sets the is_list_item of this ListFormat.
 
-        Gets or sets the list level number (0 to 8) for the paragraph.  # noqa: E501
+        Gets or sets a value indicating whether the paragraph has bulleted or numbered formatting applied to it.  # noqa: E501
 
-        :param list_level_number: The list_level_number of this ListFormat.  # noqa: E501
-        :type: int
+        :param is_list_item: The is_list_item of this ListFormat.  # noqa: E501
+        :type: bool
         """
-        self._list_level_number = list_level_number
+        self._is_list_item = is_list_item
 
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/header_footer_link_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/header_footer_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,38 +39,38 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'data': 'str',
-        'id': 'str'
+        'id': 'str',
+        'data': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
-        'data': 'Data',
-        'id': 'Id'
+        'id': 'Id',
+        'data': 'Data'
     }
 
-    def __init__(self, link=None, data=None, id=None):  # noqa: E501
+    def __init__(self, link=None, id=None, data=None):  # noqa: E501
         """CustomXmlPart - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._data = None
         self._id = None
+        self._data = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if data is not None:
-            self.data = data
         if id is not None:
             self.id = id
+        if data is not None:
+            self.data = data
 
     @property
     def link(self):
         """Gets the link of this CustomXmlPart.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -87,36 +87,14 @@
 
         :param link: The link of this CustomXmlPart.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def data(self):
-        """Gets the data of this CustomXmlPart.  # noqa: E501
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :return: The data of this CustomXmlPart.  # noqa: E501
-        :rtype: str
-        """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this CustomXmlPart.
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :param data: The data of this CustomXmlPart.  # noqa: E501
-        :type: str
-        """
-        self._data = data
-
-    @property
     def id(self):
         """Gets the id of this CustomXmlPart.  # noqa: E501
 
         Gets or sets the custom xml part id.  # noqa: E501
 
         :return: The id of this CustomXmlPart.  # noqa: E501
         :rtype: str
@@ -130,14 +108,36 @@
         Gets or sets the custom xml part id.  # noqa: E501
 
         :param id: The id of this CustomXmlPart.  # noqa: E501
         :type: str
         """
         self._id = id
 
+    @property
+    def data(self):
+        """Gets the data of this CustomXmlPart.  # noqa: E501
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :return: The data of this CustomXmlPart.  # noqa: E501
+        :rtype: str
+        """
+        return self._data
+
+    @data.setter
+    def data(self, data):
+        """Sets the data of this CustomXmlPart.
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :param data: The data of this CustomXmlPart.  # noqa: E501
+        :type: str
+        """
+        self._data = data
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/pcl_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/pcl_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/preferred_width.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/preferred_width.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/error_details.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/text_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/text_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         'encoding': 'str',
         'export_headers_footers_mode': 'str',
         'force_page_breaks': 'bool',
         'paragraph_break': 'str',
         'add_bidi_marks': 'bool',
         'max_characters_per_line': 'int',
         'preserve_table_layout': 'bool',
-        'save_format': 'str',
-        'simplify_list_labels': 'bool'
+        'simplify_list_labels': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -83,16 +83,16 @@
         'encoding': 'Encoding',
         'export_headers_footers_mode': 'ExportHeadersFootersMode',
         'force_page_breaks': 'ForcePageBreaks',
         'paragraph_break': 'ParagraphBreak',
         'add_bidi_marks': 'AddBidiMarks',
         'max_characters_per_line': 'MaxCharactersPerLine',
         'preserve_table_layout': 'PreserveTableLayout',
-        'save_format': 'SaveFormat',
-        'simplify_list_labels': 'SimplifyListLabels'
+        'simplify_list_labels': 'SimplifyListLabels',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, encoding=None, export_headers_footers_mode=None, force_page_breaks=None, paragraph_break=None, add_bidi_marks=None, max_characters_per_line=None, preserve_table_layout=None, simplify_list_labels=None):  # noqa: E501
         """TextSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -110,16 +110,16 @@
         self._encoding = None
         self._export_headers_footers_mode = None
         self._force_page_breaks = None
         self._paragraph_break = None
         self._add_bidi_marks = None
         self._max_characters_per_line = None
         self._preserve_table_layout = None
-        self._save_format = "txt"
         self._simplify_list_labels = None
+        self._save_format = "txt"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -638,26 +638,14 @@
 
         :param preserve_table_layout: The preserve_table_layout of this TextSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._preserve_table_layout = preserve_table_layout
 
     @property
-    def save_format(self):
-        """Gets the save_format of this TextSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this TextSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def simplify_list_labels(self):
         """Gets the simplify_list_labels of this TextSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating whether the program should simplify list labels in case of complex label formatting not being adequately represented by plain text.  # noqa: E501
 
         :return: The simplify_list_labels of this TextSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -671,14 +659,26 @@
         Gets or sets a value indicating whether the program should simplify list labels in case of complex label formatting not being adequately represented by plain text.  # noqa: E501
 
         :param simplify_list_labels: The simplify_list_labels of this TextSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._simplify_list_labels = simplify_list_labels
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this TextSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this TextSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/font.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/border_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/border_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_properties_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_cell_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_cell_insert.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/structured_document_tag_list_item.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/structured_document_tag_list_item.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/font_info.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/font_info.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_names.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_names.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section_link_collection.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link_collection.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/custom_xml_part_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/custom_xml_part_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,38 +39,38 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
-        'data': 'str',
-        'id': 'str'
+        'id': 'str',
+        'data': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
-        'data': 'Data',
-        'id': 'Id'
+        'id': 'Id',
+        'data': 'Data'
     }
 
-    def __init__(self, link=None, data=None, id=None):  # noqa: E501
+    def __init__(self, link=None, id=None, data=None):  # noqa: E501
         """CustomXmlPartInsert - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
-        self._data = None
         self._id = None
+        self._data = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
-        if data is not None:
-            self.data = data
         if id is not None:
             self.id = id
+        if data is not None:
+            self.data = data
 
     @property
     def link(self):
         """Gets the link of this CustomXmlPartInsert.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -87,36 +87,14 @@
 
         :param link: The link of this CustomXmlPartInsert.  # noqa: E501
         :type: WordsApiLink
         """
         self._link = link
 
     @property
-    def data(self):
-        """Gets the data of this CustomXmlPartInsert.  # noqa: E501
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :return: The data of this CustomXmlPartInsert.  # noqa: E501
-        :rtype: str
-        """
-        return self._data
-
-    @data.setter
-    def data(self, data):
-        """Sets the data of this CustomXmlPartInsert.
-
-        Gets or sets the custom xml part data.  # noqa: E501
-
-        :param data: The data of this CustomXmlPartInsert.  # noqa: E501
-        :type: str
-        """
-        self._data = data
-
-    @property
     def id(self):
         """Gets the id of this CustomXmlPartInsert.  # noqa: E501
 
         Gets or sets the custom xml part id.  # noqa: E501
 
         :return: The id of this CustomXmlPartInsert.  # noqa: E501
         :rtype: str
@@ -130,14 +108,36 @@
         Gets or sets the custom xml part id.  # noqa: E501
 
         :param id: The id of this CustomXmlPartInsert.  # noqa: E501
         :type: str
         """
         self._id = id
 
+    @property
+    def data(self):
+        """Gets the data of this CustomXmlPartInsert.  # noqa: E501
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :return: The data of this CustomXmlPartInsert.  # noqa: E501
+        :rtype: str
+        """
+        return self._data
+
+    @data.setter
+    def data(self, data):
+        """Sets the data of this CustomXmlPartInsert.
+
+        Gets or sets the custom xml part data.  # noqa: E501
+
+        :param data: The data of this CustomXmlPartInsert.  # noqa: E501
+        :type: str
+        """
+        self._data = data
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/storage_file.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnotes_stat_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnotes_stat_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,42 +40,42 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'row_format': 'TableRowFormat',
-        'table_cell_list': 'list[TableCell]'
+        'table_cell_list': 'list[TableCell]',
+        'row_format': 'TableRowFormat'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'row_format': 'RowFormat',
-        'table_cell_list': 'TableCellList'
+        'table_cell_list': 'TableCellList',
+        'row_format': 'RowFormat'
     }
 
-    def __init__(self, link=None, node_id=None, row_format=None, table_cell_list=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, table_cell_list=None, row_format=None):  # noqa: E501
         """TableRow - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._row_format = None
         self._table_cell_list = None
+        self._row_format = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if row_format is not None:
-            self.row_format = row_format
         if table_cell_list is not None:
             self.table_cell_list = table_cell_list
+        if row_format is not None:
+            self.row_format = row_format
 
     @property
     def link(self):
         """Gets the link of this TableRow.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -114,36 +114,14 @@
 
         :param node_id: The node_id of this TableRow.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def row_format(self):
-        """Gets the row_format of this TableRow.  # noqa: E501
-
-        Gets or sets the formatting properties of a row.  # noqa: E501
-
-        :return: The row_format of this TableRow.  # noqa: E501
-        :rtype: TableRowFormat
-        """
-        return self._row_format
-
-    @row_format.setter
-    def row_format(self, row_format):
-        """Sets the row_format of this TableRow.
-
-        Gets or sets the formatting properties of a row.  # noqa: E501
-
-        :param row_format: The row_format of this TableRow.  # noqa: E501
-        :type: TableRowFormat
-        """
-        self._row_format = row_format
-
-    @property
     def table_cell_list(self):
         """Gets the table_cell_list of this TableRow.  # noqa: E501
 
         Gets or sets the collection of rows.  # noqa: E501
 
         :return: The table_cell_list of this TableRow.  # noqa: E501
         :rtype: list[TableCell]
@@ -157,14 +135,36 @@
         Gets or sets the collection of rows.  # noqa: E501
 
         :param table_cell_list: The table_cell_list of this TableRow.  # noqa: E501
         :type: list[TableCell]
         """
         self._table_cell_list = table_cell_list
 
+    @property
+    def row_format(self):
+        """Gets the row_format of this TableRow.  # noqa: E501
+
+        Gets or sets the formatting properties of a row.  # noqa: E501
+
+        :return: The row_format of this TableRow.  # noqa: E501
+        :rtype: TableRowFormat
+        """
+        return self._row_format
+
+    @row_format.setter
+    def row_format(self, row_format):
+        """Sets the row_format of this TableRow.
+
+        Gets or sets the formatting properties of a row.  # noqa: E501
+
+        :param row_format: The row_format of this TableRow.  # noqa: E501
+        :type: TableRowFormat
+        """
+        self._row_format = row_format
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/field_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/field_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/doc_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/doc_save_options_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         'update_fields': 'bool',
         'update_last_printed_property': 'bool',
         'update_last_saved_time_property': 'bool',
         'update_sdt_content': 'bool',
         'zip_output': 'bool',
         'always_compress_metafiles': 'bool',
         'password': 'str',
-        'save_format': 'str',
         'save_picture_bullet': 'bool',
-        'save_routing_slip': 'bool'
+        'save_routing_slip': 'bool',
+        'save_format': 'str'
     }
 
     attribute_map = {
         'allow_embedding_post_script_fonts': 'AllowEmbeddingPostScriptFonts',
         'custom_time_zone_info_data': 'CustomTimeZoneInfoData',
         'dml3_d_effects_rendering_mode': 'Dml3DEffectsRenderingMode',
         'dml_effects_rendering_mode': 'DmlEffectsRenderingMode',
@@ -74,17 +74,17 @@
         'update_fields': 'UpdateFields',
         'update_last_printed_property': 'UpdateLastPrintedProperty',
         'update_last_saved_time_property': 'UpdateLastSavedTimeProperty',
         'update_sdt_content': 'UpdateSdtContent',
         'zip_output': 'ZipOutput',
         'always_compress_metafiles': 'AlwaysCompressMetafiles',
         'password': 'Password',
-        'save_format': 'SaveFormat',
         'save_picture_bullet': 'SavePictureBullet',
-        'save_routing_slip': 'SaveRoutingSlip'
+        'save_routing_slip': 'SaveRoutingSlip',
+        'save_format': 'SaveFormat'
     }
 
     def __init__(self, allow_embedding_post_script_fonts=None, custom_time_zone_info_data=None, dml3_d_effects_rendering_mode=None, dml_effects_rendering_mode=None, dml_rendering_mode=None, file_name=None, iml_rendering_mode=None, update_created_time_property=None, update_fields=None, update_last_printed_property=None, update_last_saved_time_property=None, update_sdt_content=None, zip_output=None, always_compress_metafiles=None, password=None, save_picture_bullet=None, save_routing_slip=None):  # noqa: E501
         """DocSaveOptionsData - a model defined in Swagger"""  # noqa: E501
 
         self._allow_embedding_post_script_fonts = None
         self._custom_time_zone_info_data = None
@@ -97,17 +97,17 @@
         self._update_fields = None
         self._update_last_printed_property = None
         self._update_last_saved_time_property = None
         self._update_sdt_content = None
         self._zip_output = None
         self._always_compress_metafiles = None
         self._password = None
-        self._save_format = "doc"
         self._save_picture_bullet = None
         self._save_routing_slip = None
+        self._save_format = "doc"
         self.discriminator = None
 
         if allow_embedding_post_script_fonts is not None:
             self.allow_embedding_post_script_fonts = allow_embedding_post_script_fonts
         if custom_time_zone_info_data is not None:
             self.custom_time_zone_info_data = custom_time_zone_info_data
         if dml3_d_effects_rendering_mode is not None:
@@ -500,26 +500,14 @@
 
         :param password: The password of this DocSaveOptionsData.  # noqa: E501
         :type: str
         """
         self._password = password
 
     @property
-    def save_format(self):
-        """Gets the save_format of this DocSaveOptionsData.  # noqa: E501
-
-        Gets the format of save.  # noqa: E501
-
-        :return: The save_format of this DocSaveOptionsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._save_format
-
-
-    @property
     def save_picture_bullet(self):
         """Gets the save_picture_bullet of this DocSaveOptionsData.  # noqa: E501
 
         Gets or sets a value indicating when False, that PictureBullet data is not saved to the output document. The default value is true.  # noqa: E501
 
         :return: The save_picture_bullet of this DocSaveOptionsData.  # noqa: E501
         :rtype: bool
@@ -555,14 +543,26 @@
         Gets or sets a value indicating whether to save RoutingSlip data to output document.  # noqa: E501
 
         :param save_routing_slip: The save_routing_slip of this DocSaveOptionsData.  # noqa: E501
         :type: bool
         """
         self._save_routing_slip = save_routing_slip
 
+    @property
+    def save_format(self):
+        """Gets the save_format of this DocSaveOptionsData.  # noqa: E501
+
+        Gets the format of save.  # noqa: E501
+
+        :return: The save_format of this DocSaveOptionsData.  # noqa: E501
+        :rtype: str
+        """
+        return self._save_format
+
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/hyperlink.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_permissions.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_permissions.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/page_number.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/page_number.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/files_list.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/api_error.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/api_error.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_properties_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_properties_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/available_fonts_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/available_fonts_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/table_row_format_dto.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/table_row_format_dto.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/search_result.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/search_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,56 +38,34 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'range_end': 'DocumentPosition',
-        'range_start': 'DocumentPosition'
+        'range_start': 'DocumentPosition',
+        'range_end': 'DocumentPosition'
     }
 
     attribute_map = {
-        'range_end': 'RangeEnd',
-        'range_start': 'RangeStart'
+        'range_start': 'RangeStart',
+        'range_end': 'RangeEnd'
     }
 
-    def __init__(self, range_end=None, range_start=None):  # noqa: E501
+    def __init__(self, range_start=None, range_end=None):  # noqa: E501
         """SearchResult - a model defined in Swagger"""  # noqa: E501
 
-        self._range_end = None
         self._range_start = None
+        self._range_end = None
         self.discriminator = None
 
-        if range_end is not None:
-            self.range_end = range_end
         if range_start is not None:
             self.range_start = range_start
-
-    @property
-    def range_end(self):
-        """Gets the range_end of this SearchResult.  # noqa: E501
-
-        Gets or sets the link to result range end node.  # noqa: E501
-
-        :return: The range_end of this SearchResult.  # noqa: E501
-        :rtype: DocumentPosition
-        """
-        return self._range_end
-
-    @range_end.setter
-    def range_end(self, range_end):
-        """Sets the range_end of this SearchResult.
-
-        Gets or sets the link to result range end node.  # noqa: E501
-
-        :param range_end: The range_end of this SearchResult.  # noqa: E501
-        :type: DocumentPosition
-        """
-        self._range_end = range_end
+        if range_end is not None:
+            self.range_end = range_end
 
     @property
     def range_start(self):
         """Gets the range_start of this SearchResult.  # noqa: E501
 
         Gets or sets the link to result range start node.  # noqa: E501
 
@@ -103,14 +81,36 @@
         Gets or sets the link to result range start node.  # noqa: E501
 
         :param range_start: The range_start of this SearchResult.  # noqa: E501
         :type: DocumentPosition
         """
         self._range_start = range_start
 
+    @property
+    def range_end(self):
+        """Gets the range_end of this SearchResult.  # noqa: E501
+
+        Gets or sets the link to result range end node.  # noqa: E501
+
+        :return: The range_end of this SearchResult.  # noqa: E501
+        :rtype: DocumentPosition
+        """
+        return self._range_end
+
+    @range_end.setter
+    def range_end(self, range_end):
+        """Sets the range_end of this SearchResult.
+
+        Gets or sets the link to result range end node.  # noqa: E501
+
+        :param range_end: The range_end of this SearchResult.  # noqa: E501
+        :type: DocumentPosition
+        """
+        self._range_end = range_end
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/page_stat_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/page_stat_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,43 +39,43 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'footnotes_stat_data': 'FootnotesStatData',
-        'page_number': 'int',
         'paragraph_count': 'int',
-        'word_count': 'int'
+        'word_count': 'int',
+        'page_number': 'int'
     }
 
     attribute_map = {
         'footnotes_stat_data': 'FootnotesStatData',
-        'page_number': 'PageNumber',
         'paragraph_count': 'ParagraphCount',
-        'word_count': 'WordCount'
+        'word_count': 'WordCount',
+        'page_number': 'PageNumber'
     }
 
-    def __init__(self, footnotes_stat_data=None, page_number=None, paragraph_count=None, word_count=None):  # noqa: E501
+    def __init__(self, footnotes_stat_data=None, paragraph_count=None, word_count=None, page_number=None):  # noqa: E501
         """PageStatData - a model defined in Swagger"""  # noqa: E501
 
         self._footnotes_stat_data = None
-        self._page_number = None
         self._paragraph_count = None
         self._word_count = None
+        self._page_number = None
         self.discriminator = None
 
         if footnotes_stat_data is not None:
             self.footnotes_stat_data = footnotes_stat_data
-        if page_number is not None:
-            self.page_number = page_number
         if paragraph_count is not None:
             self.paragraph_count = paragraph_count
         if word_count is not None:
             self.word_count = word_count
+        if page_number is not None:
+            self.page_number = page_number
 
     @property
     def footnotes_stat_data(self):
         """Gets the footnotes_stat_data of this PageStatData.  # noqa: E501
 
         Gets or sets the detailed statistics on the footnotes.  # noqa: E501
 
@@ -92,36 +92,14 @@
 
         :param footnotes_stat_data: The footnotes_stat_data of this PageStatData.  # noqa: E501
         :type: FootnotesStatData
         """
         self._footnotes_stat_data = footnotes_stat_data
 
     @property
-    def page_number(self):
-        """Gets the page_number of this PageStatData.  # noqa: E501
-
-        Gets or sets the page number.  # noqa: E501
-
-        :return: The page_number of this PageStatData.  # noqa: E501
-        :rtype: int
-        """
-        return self._page_number
-
-    @page_number.setter
-    def page_number(self, page_number):
-        """Sets the page_number of this PageStatData.
-
-        Gets or sets the page number.  # noqa: E501
-
-        :param page_number: The page_number of this PageStatData.  # noqa: E501
-        :type: int
-        """
-        self._page_number = page_number
-
-    @property
     def paragraph_count(self):
         """Gets the paragraph_count of this PageStatData.  # noqa: E501
 
         Gets or sets the total count of paragraphs in the page.  # noqa: E501
 
         :return: The paragraph_count of this PageStatData.  # noqa: E501
         :rtype: int
@@ -157,14 +135,36 @@
         Gets or sets the total count of words in the page.  # noqa: E501
 
         :param word_count: The word_count of this PageStatData.  # noqa: E501
         :type: int
         """
         self._word_count = word_count
 
+    @property
+    def page_number(self):
+        """Gets the page_number of this PageStatData.  # noqa: E501
+
+        Gets or sets the page number.  # noqa: E501
+
+        :return: The page_number of this PageStatData.  # noqa: E501
+        :rtype: int
+        """
+        return self._page_number
+
+    @page_number.setter
+    def page_number(self, page_number):
+        """Sets the page_number of this PageStatData.
+
+        Gets or sets the page number.  # noqa: E501
+
+        :param page_number: The page_number of this PageStatData.  # noqa: E501
+        :type: int
+        """
+        self._page_number = page_number
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/xaml_flow_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/xaml_flow_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/json_data_load_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/json_data_load_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/section_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/section_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/compress_options.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/compress_options.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/mhtml_save_options_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/mhtml_save_options_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/run.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/run.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/words_response.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/words_response.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/footnote.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/footnote.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,57 +40,57 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'content': 'StoryChildNodes',
-        'footnote_type': 'str',
         'position': 'DocumentPosition',
+        'footnote_type': 'str',
         'reference_mark': 'str',
-        'text': 'str'
+        'text': 'str',
+        'content': 'StoryChildNodes'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'content': 'Content',
-        'footnote_type': 'FootnoteType',
         'position': 'Position',
+        'footnote_type': 'FootnoteType',
         'reference_mark': 'ReferenceMark',
-        'text': 'Text'
+        'text': 'Text',
+        'content': 'Content'
     }
 
-    def __init__(self, link=None, node_id=None, content=None, footnote_type=None, position=None, reference_mark=None, text=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, position=None, footnote_type=None, reference_mark=None, text=None, content=None):  # noqa: E501
         """Footnote - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._content = None
-        self._footnote_type = None
         self._position = None
+        self._footnote_type = None
         self._reference_mark = None
         self._text = None
+        self._content = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if content is not None:
-            self.content = content
-        if footnote_type is not None:
-            self.footnote_type = footnote_type
         if position is not None:
             self.position = position
+        if footnote_type is not None:
+            self.footnote_type = footnote_type
         if reference_mark is not None:
             self.reference_mark = reference_mark
         if text is not None:
             self.text = text
+        if content is not None:
+            self.content = content
 
     @property
     def link(self):
         """Gets the link of this Footnote.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -129,34 +129,34 @@
 
         :param node_id: The node_id of this Footnote.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def content(self):
-        """Gets the content of this Footnote.  # noqa: E501
+    def position(self):
+        """Gets the position of this Footnote.  # noqa: E501
 
-        Gets or sets the content of the footnote.  # noqa: E501
+        Gets or sets the link to comment range start node.  # noqa: E501
 
-        :return: The content of this Footnote.  # noqa: E501
-        :rtype: StoryChildNodes
+        :return: The position of this Footnote.  # noqa: E501
+        :rtype: DocumentPosition
         """
-        return self._content
+        return self._position
 
-    @content.setter
-    def content(self, content):
-        """Sets the content of this Footnote.
+    @position.setter
+    def position(self, position):
+        """Sets the position of this Footnote.
 
-        Gets or sets the content of the footnote.  # noqa: E501
+        Gets or sets the link to comment range start node.  # noqa: E501
 
-        :param content: The content of this Footnote.  # noqa: E501
-        :type: StoryChildNodes
+        :param position: The position of this Footnote.  # noqa: E501
+        :type: DocumentPosition
         """
-        self._content = content
+        self._position = position
 
     @property
     def footnote_type(self):
         """Gets the footnote_type of this Footnote.  # noqa: E501
 
         Gets or sets the value, that specifies whether this is a footnote or endnote.  # noqa: E501
 
@@ -181,36 +181,14 @@
                     "Invalid value for `footnote_type` ({0}), must be one of {1}"  # noqa: E501
                     .format(footnote_type, allowed_values))
             self._footnote_type = footnote_type
         else:
             self._footnote_type = allowed_values[int(footnote_type) if six.PY3 else long(footnote_type)]
 
     @property
-    def position(self):
-        """Gets the position of this Footnote.  # noqa: E501
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :return: The position of this Footnote.  # noqa: E501
-        :rtype: DocumentPosition
-        """
-        return self._position
-
-    @position.setter
-    def position(self, position):
-        """Sets the position of this Footnote.
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :param position: The position of this Footnote.  # noqa: E501
-        :type: DocumentPosition
-        """
-        self._position = position
-
-    @property
     def reference_mark(self):
         """Gets the reference_mark of this Footnote.  # noqa: E501
 
         Gets or sets the custom reference mark to be used for this footnote. Default value is Empty, meaning auto-numbered footnotes are used.  # noqa: E501
 
         :return: The reference_mark of this Footnote.  # noqa: E501
         :rtype: str
@@ -246,14 +224,36 @@
         Gets or sets text of the footnote.  # noqa: E501
 
         :param text: The text of this Footnote.  # noqa: E501
         :type: str
         """
         self._text = text
 
+    @property
+    def content(self):
+        """Gets the content of this Footnote.  # noqa: E501
+
+        Gets or sets the content of the footnote.  # noqa: E501
+
+        :return: The content of this Footnote.  # noqa: E501
+        :rtype: StoryChildNodes
+        """
+        return self._content
+
+    @content.setter
+    def content(self, content):
+        """Sets the content of this Footnote.
+
+        Gets or sets the content of the footnote.  # noqa: E501
+
+        :param content: The content of this Footnote.  # noqa: E501
+        :type: StoryChildNodes
+        """
+        self._content = content
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/link_element.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/pdf_encryption_details_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/pdf_encryption_details_data.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/comment_insert.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/comment_insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,56 +38,100 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'range_start': 'NewDocumentPosition',
+        'range_end': 'NewDocumentPosition',
         'author': 'str',
         'date_time': 'datetime',
         'initial': 'str',
-        'range_end': 'NewDocumentPosition',
-        'range_start': 'NewDocumentPosition',
         'text': 'str'
     }
 
     attribute_map = {
+        'range_start': 'RangeStart',
+        'range_end': 'RangeEnd',
         'author': 'Author',
         'date_time': 'DateTime',
         'initial': 'Initial',
-        'range_end': 'RangeEnd',
-        'range_start': 'RangeStart',
         'text': 'Text'
     }
 
-    def __init__(self, author=None, date_time=None, initial=None, range_end=None, range_start=None, text=None):  # noqa: E501
+    def __init__(self, range_start=None, range_end=None, author=None, date_time=None, initial=None, text=None):  # noqa: E501
         """CommentInsert - a model defined in Swagger"""  # noqa: E501
 
+        self._range_start = None
+        self._range_end = None
         self._author = None
         self._date_time = None
         self._initial = None
-        self._range_end = None
-        self._range_start = None
         self._text = None
         self.discriminator = None
 
+        if range_start is not None:
+            self.range_start = range_start
+        if range_end is not None:
+            self.range_end = range_end
         if author is not None:
             self.author = author
         if date_time is not None:
             self.date_time = date_time
         if initial is not None:
             self.initial = initial
-        if range_end is not None:
-            self.range_end = range_end
-        if range_start is not None:
-            self.range_start = range_start
         if text is not None:
             self.text = text
 
     @property
+    def range_start(self):
+        """Gets the range_start of this CommentInsert.  # noqa: E501
+
+        Gets or sets the link to comment range start node.  # noqa: E501
+
+        :return: The range_start of this CommentInsert.  # noqa: E501
+        :rtype: NewDocumentPosition
+        """
+        return self._range_start
+
+    @range_start.setter
+    def range_start(self, range_start):
+        """Sets the range_start of this CommentInsert.
+
+        Gets or sets the link to comment range start node.  # noqa: E501
+
+        :param range_start: The range_start of this CommentInsert.  # noqa: E501
+        :type: NewDocumentPosition
+        """
+        self._range_start = range_start
+
+    @property
+    def range_end(self):
+        """Gets the range_end of this CommentInsert.  # noqa: E501
+
+        Gets or sets the link to comment range end node.  # noqa: E501
+
+        :return: The range_end of this CommentInsert.  # noqa: E501
+        :rtype: NewDocumentPosition
+        """
+        return self._range_end
+
+    @range_end.setter
+    def range_end(self, range_end):
+        """Sets the range_end of this CommentInsert.
+
+        Gets or sets the link to comment range end node.  # noqa: E501
+
+        :param range_end: The range_end of this CommentInsert.  # noqa: E501
+        :type: NewDocumentPosition
+        """
+        self._range_end = range_end
+
+    @property
     def author(self):
         """Gets the author of this CommentInsert.  # noqa: E501
 
         Gets or sets the author name for a comment.  # noqa: E501
 
         :return: The author of this CommentInsert.  # noqa: E501
         :rtype: str
@@ -146,58 +190,14 @@
 
         :param initial: The initial of this CommentInsert.  # noqa: E501
         :type: str
         """
         self._initial = initial
 
     @property
-    def range_end(self):
-        """Gets the range_end of this CommentInsert.  # noqa: E501
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :return: The range_end of this CommentInsert.  # noqa: E501
-        :rtype: NewDocumentPosition
-        """
-        return self._range_end
-
-    @range_end.setter
-    def range_end(self, range_end):
-        """Sets the range_end of this CommentInsert.
-
-        Gets or sets the link to comment range end node.  # noqa: E501
-
-        :param range_end: The range_end of this CommentInsert.  # noqa: E501
-        :type: NewDocumentPosition
-        """
-        self._range_end = range_end
-
-    @property
-    def range_start(self):
-        """Gets the range_start of this CommentInsert.  # noqa: E501
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :return: The range_start of this CommentInsert.  # noqa: E501
-        :rtype: NewDocumentPosition
-        """
-        return self._range_start
-
-    @range_start.setter
-    def range_start(self, range_start):
-        """Sets the range_start of this CommentInsert.
-
-        Gets or sets the link to comment range start node.  # noqa: E501
-
-        :param range_start: The range_start of this CommentInsert.  # noqa: E501
-        :type: NewDocumentPosition
-        """
-        self._range_start = range_start
-
-    @property
     def text(self):
         """Gets the text of this CommentInsert.  # noqa: E501
 
         Gets or sets text of the comment.  # noqa: E501
 
         :return: The text of this CommentInsert.  # noqa: E501
         :rtype: str
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/office_math_link.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/office_math_link.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_entry_list.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_entry_list.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/form_field.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/form_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,77 +40,77 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'link': 'WordsApiLink',
         'node_id': 'str',
-        'calculate_on_exit': 'bool',
+        'name': 'str',
         'enabled': 'bool',
-        'entry_macro': 'str',
-        'exit_macro': 'str',
+        'status_text': 'str',
+        'own_status': 'bool',
         'help_text': 'str',
-        'name': 'str',
         'own_help': 'bool',
-        'own_status': 'bool',
-        'status_text': 'str'
+        'calculate_on_exit': 'bool',
+        'entry_macro': 'str',
+        'exit_macro': 'str'
     }
 
     attribute_map = {
         'link': 'Link',
         'node_id': 'NodeId',
-        'calculate_on_exit': 'CalculateOnExit',
+        'name': 'Name',
         'enabled': 'Enabled',
-        'entry_macro': 'EntryMacro',
-        'exit_macro': 'ExitMacro',
+        'status_text': 'StatusText',
+        'own_status': 'OwnStatus',
         'help_text': 'HelpText',
-        'name': 'Name',
         'own_help': 'OwnHelp',
-        'own_status': 'OwnStatus',
-        'status_text': 'StatusText'
+        'calculate_on_exit': 'CalculateOnExit',
+        'entry_macro': 'EntryMacro',
+        'exit_macro': 'ExitMacro'
     }
 
-    def __init__(self, link=None, node_id=None, calculate_on_exit=None, enabled=None, entry_macro=None, exit_macro=None, help_text=None, name=None, own_help=None, own_status=None, status_text=None):  # noqa: E501
+    def __init__(self, link=None, node_id=None, name=None, enabled=None, status_text=None, own_status=None, help_text=None, own_help=None, calculate_on_exit=None, entry_macro=None, exit_macro=None):  # noqa: E501
         """FormField - a model defined in Swagger"""  # noqa: E501
 
         self._link = None
         self._node_id = None
-        self._calculate_on_exit = None
+        self._name = None
         self._enabled = None
-        self._entry_macro = None
-        self._exit_macro = None
+        self._status_text = None
+        self._own_status = None
         self._help_text = None
-        self._name = None
         self._own_help = None
-        self._own_status = None
-        self._status_text = None
+        self._calculate_on_exit = None
+        self._entry_macro = None
+        self._exit_macro = None
         self.discriminator = None
 
         if link is not None:
             self.link = link
         if node_id is not None:
             self.node_id = node_id
-        if calculate_on_exit is not None:
-            self.calculate_on_exit = calculate_on_exit
+        if name is not None:
+            self.name = name
         if enabled is not None:
             self.enabled = enabled
-        if entry_macro is not None:
-            self.entry_macro = entry_macro
-        if exit_macro is not None:
-            self.exit_macro = exit_macro
+        if status_text is not None:
+            self.status_text = status_text
+        if own_status is not None:
+            self.own_status = own_status
         if help_text is not None:
             self.help_text = help_text
-        if name is not None:
-            self.name = name
         if own_help is not None:
             self.own_help = own_help
-        if own_status is not None:
-            self.own_status = own_status
-        if status_text is not None:
-            self.status_text = status_text
+        if calculate_on_exit is not None:
+            self.calculate_on_exit = calculate_on_exit
+        if entry_macro is not None:
+            self.entry_macro = entry_macro
+        if exit_macro is not None:
+            self.exit_macro = exit_macro
 
     @property
     def link(self):
         """Gets the link of this FormField.  # noqa: E501
 
         Gets or sets the link to the document.  # noqa: E501
 
@@ -149,34 +149,34 @@
 
         :param node_id: The node_id of this FormField.  # noqa: E501
         :type: str
         """
         self._node_id = node_id
 
     @property
-    def calculate_on_exit(self):
-        """Gets the calculate_on_exit of this FormField.  # noqa: E501
+    def name(self):
+        """Gets the name of this FormField.  # noqa: E501
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :return: The calculate_on_exit of this FormField.  # noqa: E501
-        :rtype: bool
+        :return: The name of this FormField.  # noqa: E501
+        :rtype: str
         """
-        return self._calculate_on_exit
+        return self._name
 
-    @calculate_on_exit.setter
-    def calculate_on_exit(self, calculate_on_exit):
-        """Sets the calculate_on_exit of this FormField.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this FormField.
 
-        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
+        Gets or sets the form field name.  # noqa: E501
 
-        :param calculate_on_exit: The calculate_on_exit of this FormField.  # noqa: E501
-        :type: bool
+        :param name: The name of this FormField.  # noqa: E501
+        :type: str
         """
-        self._calculate_on_exit = calculate_on_exit
+        self._name = name
 
     @property
     def enabled(self):
         """Gets the enabled of this FormField.  # noqa: E501
 
         Gets or sets a value indicating whether a form field is enabled.  # noqa: E501
 
@@ -193,56 +193,56 @@
 
         :param enabled: The enabled of this FormField.  # noqa: E501
         :type: bool
         """
         self._enabled = enabled
 
     @property
-    def entry_macro(self):
-        """Gets the entry_macro of this FormField.  # noqa: E501
+    def status_text(self):
+        """Gets the status_text of this FormField.  # noqa: E501
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The entry_macro of this FormField.  # noqa: E501
+        :return: The status_text of this FormField.  # noqa: E501
         :rtype: str
         """
-        return self._entry_macro
+        return self._status_text
 
-    @entry_macro.setter
-    def entry_macro(self, entry_macro):
-        """Sets the entry_macro of this FormField.
+    @status_text.setter
+    def status_text(self, status_text):
+        """Sets the status_text of this FormField.
 
-        Gets or sets the entry macro name for the form field.  # noqa: E501
+        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param entry_macro: The entry_macro of this FormField.  # noqa: E501
+        :param status_text: The status_text of this FormField.  # noqa: E501
         :type: str
         """
-        self._entry_macro = entry_macro
+        self._status_text = status_text
 
     @property
-    def exit_macro(self):
-        """Gets the exit_macro of this FormField.  # noqa: E501
+    def own_status(self):
+        """Gets the own_status of this FormField.  # noqa: E501
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :return: The exit_macro of this FormField.  # noqa: E501
-        :rtype: str
+        :return: The own_status of this FormField.  # noqa: E501
+        :rtype: bool
         """
-        return self._exit_macro
+        return self._own_status
 
-    @exit_macro.setter
-    def exit_macro(self, exit_macro):
-        """Sets the exit_macro of this FormField.
+    @own_status.setter
+    def own_status(self, own_status):
+        """Sets the own_status of this FormField.
 
-        Gets or sets the exit macro name for the form field.  # noqa: E501
+        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
 
-        :param exit_macro: The exit_macro of this FormField.  # noqa: E501
-        :type: str
+        :param own_status: The own_status of this FormField.  # noqa: E501
+        :type: bool
         """
-        self._exit_macro = exit_macro
+        self._own_status = own_status
 
     @property
     def help_text(self):
         """Gets the help_text of this FormField.  # noqa: E501
 
         Gets or sets text, displayed in a message box when the form field has the focus and the user presses F1.  # noqa: E501
 
@@ -259,36 +259,14 @@
 
         :param help_text: The help_text of this FormField.  # noqa: E501
         :type: str
         """
         self._help_text = help_text
 
     @property
-    def name(self):
-        """Gets the name of this FormField.  # noqa: E501
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :return: The name of this FormField.  # noqa: E501
-        :rtype: str
-        """
-        return self._name
-
-    @name.setter
-    def name(self, name):
-        """Sets the name of this FormField.
-
-        Gets or sets the form field name.  # noqa: E501
-
-        :param name: The name of this FormField.  # noqa: E501
-        :type: str
-        """
-        self._name = name
-
-    @property
     def own_help(self):
         """Gets the own_help of this FormField.  # noqa: E501
 
         Gets or sets a value indicating whether the source of the text that's displayed in a message box when a form field has the focus and the user presses F1.  # noqa: E501
 
         :return: The own_help of this FormField.  # noqa: E501
         :rtype: bool
@@ -303,56 +281,78 @@
 
         :param own_help: The own_help of this FormField.  # noqa: E501
         :type: bool
         """
         self._own_help = own_help
 
     @property
-    def own_status(self):
-        """Gets the own_status of this FormField.  # noqa: E501
+    def calculate_on_exit(self):
+        """Gets the calculate_on_exit of this FormField.  # noqa: E501
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :return: The own_status of this FormField.  # noqa: E501
+        :return: The calculate_on_exit of this FormField.  # noqa: E501
         :rtype: bool
         """
-        return self._own_status
+        return self._calculate_on_exit
 
-    @own_status.setter
-    def own_status(self, own_status):
-        """Sets the own_status of this FormField.
+    @calculate_on_exit.setter
+    def calculate_on_exit(self, calculate_on_exit):
+        """Sets the calculate_on_exit of this FormField.
 
-        Gets or sets a value indicating whether the source of the text that's displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets a value indicating whether references to the specified form field are automatically updated whenever the field is exited.  # noqa: E501
 
-        :param own_status: The own_status of this FormField.  # noqa: E501
+        :param calculate_on_exit: The calculate_on_exit of this FormField.  # noqa: E501
         :type: bool
         """
-        self._own_status = own_status
+        self._calculate_on_exit = calculate_on_exit
 
     @property
-    def status_text(self):
-        """Gets the status_text of this FormField.  # noqa: E501
+    def entry_macro(self):
+        """Gets the entry_macro of this FormField.  # noqa: E501
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :return: The status_text of this FormField.  # noqa: E501
+        :return: The entry_macro of this FormField.  # noqa: E501
         :rtype: str
         """
-        return self._status_text
+        return self._entry_macro
 
-    @status_text.setter
-    def status_text(self, status_text):
-        """Sets the status_text of this FormField.
+    @entry_macro.setter
+    def entry_macro(self, entry_macro):
+        """Sets the entry_macro of this FormField.
 
-        Gets or sets text, displayed in the status bar when a form field has the focus.  # noqa: E501
+        Gets or sets the entry macro name for the form field.  # noqa: E501
 
-        :param status_text: The status_text of this FormField.  # noqa: E501
+        :param entry_macro: The entry_macro of this FormField.  # noqa: E501
         :type: str
         """
-        self._status_text = status_text
+        self._entry_macro = entry_macro
+
+    @property
+    def exit_macro(self):
+        """Gets the exit_macro of this FormField.  # noqa: E501
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :return: The exit_macro of this FormField.  # noqa: E501
+        :rtype: str
+        """
+        return self._exit_macro
+
+    @exit_macro.setter
+    def exit_macro(self, exit_macro):
+        """Sets the exit_macro of this FormField.
+
+        Gets or sets the exit macro name for the form field.  # noqa: E501
+
+        :param exit_macro: The exit_macro of this FormField.  # noqa: E501
+        :type: str
+        """
+        self._exit_macro = exit_macro
 
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/models/document_stat_data.py` & `aspose-words-cloud-23.6.0/asposewordscloud/models/document_stat_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,47 +40,47 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'footnotes_stat_data': 'FootnotesStatData',
         'page_count': 'int',
-        'page_stat_data': 'list[PageStatData]',
         'paragraph_count': 'int',
-        'word_count': 'int'
+        'word_count': 'int',
+        'page_stat_data': 'list[PageStatData]'
     }
 
     attribute_map = {
         'footnotes_stat_data': 'FootnotesStatData',
         'page_count': 'PageCount',
-        'page_stat_data': 'PageStatData',
         'paragraph_count': 'ParagraphCount',
-        'word_count': 'WordCount'
+        'word_count': 'WordCount',
+        'page_stat_data': 'PageStatData'
     }
 
-    def __init__(self, footnotes_stat_data=None, page_count=None, page_stat_data=None, paragraph_count=None, word_count=None):  # noqa: E501
+    def __init__(self, footnotes_stat_data=None, page_count=None, paragraph_count=None, word_count=None, page_stat_data=None):  # noqa: E501
         """DocumentStatData - a model defined in Swagger"""  # noqa: E501
 
         self._footnotes_stat_data = None
         self._page_count = None
-        self._page_stat_data = None
         self._paragraph_count = None
         self._word_count = None
+        self._page_stat_data = None
         self.discriminator = None
 
         if footnotes_stat_data is not None:
             self.footnotes_stat_data = footnotes_stat_data
         if page_count is not None:
             self.page_count = page_count
-        if page_stat_data is not None:
-            self.page_stat_data = page_stat_data
         if paragraph_count is not None:
             self.paragraph_count = paragraph_count
         if word_count is not None:
             self.word_count = word_count
+        if page_stat_data is not None:
+            self.page_stat_data = page_stat_data
 
     @property
     def footnotes_stat_data(self):
         """Gets the footnotes_stat_data of this DocumentStatData.  # noqa: E501
 
         Gets or sets the detailed statistics on footnotes.  # noqa: E501
 
@@ -119,36 +119,14 @@
 
         :param page_count: The page_count of this DocumentStatData.  # noqa: E501
         :type: int
         """
         self._page_count = page_count
 
     @property
-    def page_stat_data(self):
-        """Gets the page_stat_data of this DocumentStatData.  # noqa: E501
-
-        Gets or sets the detailed statistics on all pages.  # noqa: E501
-
-        :return: The page_stat_data of this DocumentStatData.  # noqa: E501
-        :rtype: list[PageStatData]
-        """
-        return self._page_stat_data
-
-    @page_stat_data.setter
-    def page_stat_data(self, page_stat_data):
-        """Sets the page_stat_data of this DocumentStatData.
-
-        Gets or sets the detailed statistics on all pages.  # noqa: E501
-
-        :param page_stat_data: The page_stat_data of this DocumentStatData.  # noqa: E501
-        :type: list[PageStatData]
-        """
-        self._page_stat_data = page_stat_data
-
-    @property
     def paragraph_count(self):
         """Gets the paragraph_count of this DocumentStatData.  # noqa: E501
 
         Gets or sets the total count of paragraphs in the document.  # noqa: E501
 
         :return: The paragraph_count of this DocumentStatData.  # noqa: E501
         :rtype: int
@@ -184,14 +162,36 @@
         Gets or sets the total count of words in the document.  # noqa: E501
 
         :param word_count: The word_count of this DocumentStatData.  # noqa: E501
         :type: int
         """
         self._word_count = word_count
 
+    @property
+    def page_stat_data(self):
+        """Gets the page_stat_data of this DocumentStatData.  # noqa: E501
+
+        Gets or sets the detailed statistics on all pages.  # noqa: E501
+
+        :return: The page_stat_data of this DocumentStatData.  # noqa: E501
+        :rtype: list[PageStatData]
+        """
+        return self._page_stat_data
+
+    @page_stat_data.setter
+    def page_stat_data(self, page_stat_data):
+        """Sets the page_stat_data of this DocumentStatData.
+
+        Gets or sets the detailed statistics on all pages.  # noqa: E501
+
+        :param page_stat_data: The page_stat_data of this DocumentStatData.  # noqa: E501
+        :type: list[PageStatData]
+        """
+        self._page_stat_data = page_stat_data
+
 
     def extract_files_content(self, filesContentResult):
         """Append the file content result list"""
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/rest.py` & `aspose-words-cloud-23.6.0/asposewordscloud/rest.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/__init__.py` & `aspose-words-cloud-23.6.0/asposewordscloud/__init__.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/configuration.py` & `aspose-words-cloud-23.6.0/asposewordscloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,10 +258,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.5\n"\
-               "SDK Package Version: 23.5".\
+               "Version of the API: 23.6\n"\
+               "SDK Package Version: 23.6".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/apis/words_api.py` & `aspose-words-cloud-23.6.0/asposewordscloud/apis/words_api.py`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/asposewordscloud/api_client.py` & `aspose-words-cloud-23.6.0/asposewordscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,20 +79,20 @@
                  cookie=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = rest.RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '23.5'}
+        self.default_headers = {'x-aspose-client': 'python sdk', 'x-aspose-version': '23.6'}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'python sdk 23.5'
+        self.user_agent = 'python sdk 23.6'
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
             self.pool.join()
 
     @property
```

### Comparing `aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/SOURCES.txt` & `aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aspose-words-cloud-23.5.1/aspose_words_cloud.egg-info/PKG-INFO` & `aspose-words-cloud-23.6.0/aspose_words_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aspose-words-cloud
-Version: 23.5.1
+Version: 23.6.0
 Summary: Python Cloud SDK wraps Aspose.Words Cloud API so you could seamlessly integrate Microsoft Word file generation, manipulation, conversion & inspection features into your own python applications.
 Home-page: https://github.com/aspose-words-cloud/aspose-words-cloud-python
 Author: Yaroslaw Ekimov
 Author-email: yaroslaw.ekimov@aspose.com
 License: UNKNOWN
 Keywords: office,convert,word,pdf,docx,html,rtf,png,jpg,split,merge,edit,word to pdf,pdf to word,docx to pdf,pdf to docx,word to html,html to word,reporting,mailmerge,statistics,watermark,fields,generate,create,report,table,paragraph,images,text,generator,creator,maker
 Platform: UNKNOWN
@@ -34,14 +34,19 @@
 - Fetch web pages via URL and save in Microsoft Word file formats.
 - Get document information in JSON or XML representation.
 - [Fetch statistical data](https://docs.aspose.cloud/display/wordscloud/Get+Document+Statistics) of a document.
 - [Remove all macros](https://docs.aspose.cloud/display/wordscloud/Remove+all+Macros+from+Document) contained in a specific document.
 - [Convert a document to desired file format](https://docs.aspose.cloud/display/wordscloud/Convert+Document+to+Destination+Format+with+Detailed+Settings+and+Save+Result+to+Storage) along with detailed settings.
 - Convert an encrypted PDF document into Word document format.
 
+## Enhancements in Version 23.6
+
+- Fix XMLHttpRequest in web applications.
+
+
 ## Enhancements in Version 23.5
 
 - Added InsertSection method.
 
 
 ## Enhancements in Version 23.4
```


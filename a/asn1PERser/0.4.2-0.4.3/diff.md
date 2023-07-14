# Comparing `tmp/asn1PERser-0.4.2.tar.gz` & `tmp/asn1PERser-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Maciej Pikula (D)\root-D\gitvobs\asn1PERser\dist\tmp720ox8\asn1PERser-0.4.2.tar", last modified: Wed Mar 29 13:22:44 2023, max compression
+gzip compressed data, was "C:\Maciej Pikula (D)\root-D\gitvobs\asn1PERser\dist\.tmp-04zv1kgs\asn1PERser-0.4.3.tar", last modified: Fri Jul 14 12:21:29 2023, max compression
```

## Comparing `asn1PERser-0.4.2.tar` & `asn1PERser-0.4.3.tar`

### file list

```diff
@@ -1,139 +1,138 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/
--rw-rw-rw-   0        0        0      435 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/assignment_def.py
--rw-rw-rw-   0        0        0     4006 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/character_and_word_set.py
--rw-rw-rw-   0        0        0     1693 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/common_def.py
--rw-rw-rw-   0        0        0     3735 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/constraint_def.py
--rw-rw-rw-   0        0        0     4475 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/lexical_items.py
--rw-rw-rw-   0        0        0     4238 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/module_def.py
--rw-rw-rw-   0        0        0    11036 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/type_def.py
--rw-rw-rw-   0        0        0     2524 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/value_def.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/asn_definitions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/data/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/
--rw-rw-rw-   0        0        0      683 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/BitStringType.py
--rw-rw-rw-   0        0        0      552 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/BooleanType.py
--rw-rw-rw-   0        0        0     1044 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/ChoiceType.py
--rw-rw-rw-   0        0        0      737 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/EnumeratedType.py
--rw-rw-rw-   0        0        0      799 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/IntegerType.py
--rw-rw-rw-   0        0        0      737 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/OctetStringType.py
--rw-rw-rw-   0        0        0     1199 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/SequenceOfType.py
--rw-rw-rw-   0        0        0     1699 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/SequenceType.py
--rw-rw-rw-   0        0        0       86 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/UTF8String.py
--rw-rw-rw-   0        0        0      364 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/builtin/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/data/__init__.py
--rw-rw-rw-   0        0        0     8636 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/module.py
--rw-rw-rw-   0        0        0     5199 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/parse_actions.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/
--rw-rw-rw-   0        0        0      704 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/creator.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/
--rw-rw-rw-   0        0        0      457 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/BitStringType.txt
--rw-rw-rw-   0        0        0       59 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/BooleanType.txt
--rw-rw-rw-   0        0        0     1898 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/ChoiceType.txt
--rw-rw-rw-   0        0        0       43 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/DefinedType.txt
--rw-rw-rw-   0        0        0      697 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/EnumeratedType.txt
--rw-rw-rw-   0        0        0      439 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/header.txt
--rw-rw-rw-   0        0        0      459 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/IntegerType.txt
--rw-rw-rw-   0        0        0      457 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/OctetStringType.txt
--rw-rw-rw-   0        0        0      507 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/SequenceOfType.txt
--rw-rw-rw-   0        0        0     3015 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/SequenceType.txt
--rw-rw-rw-   0        0        0       60 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/simple_value.txt
--rw-rw-rw-   0        0        0       46 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/type_type.txt
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/files/__init__.py
--rw-rw-rw-   0        0        0      471 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/types/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/
--rw-rw-rw-   0        0        0     1673 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/BitStringType.py
--rw-rw-rw-   0        0        0     1262 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/BooleanType.py
--rw-rw-rw-   0        0        0     5247 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/ChoiceType.py
--rw-rw-rw-   0        0        0      156 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/DateType.py
--rw-rw-rw-   0        0        0     2029 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/DefinedType.py
--rw-rw-rw-   0        0        0     2569 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/EnumeratedType.py
--rw-rw-rw-   0        0        0      175 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/IA5String.py
--rw-rw-rw-   0        0        0     1460 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/IntegerType.py
--rw-rw-rw-   0        0        0      168 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/NullType.py
--rw-rw-rw-   0        0        0      187 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/NumericString.py
--rw-rw-rw-   0        0        0     1677 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/OctetStringType.py
--rw-rw-rw-   0        0        0      168 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/RealType.py
--rw-rw-rw-   0        0        0     1989 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/SequenceOfType.py
--rw-rw-rw-   0        0        0     6204 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/SequenceType.py
--rw-rw-rw-   0        0        0      418 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/UTF8String.py
--rw-rw-rw-   0        0        0      175 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/VisibleString.py
--rw-rw-rw-   0        0        0      903 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/builtin/__init__.py
--rw-rw-rw-   0        0        0     4370 2023-03-06 10:13:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/constraint.py
--rw-rw-rw-   0        0        0     3553 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/classes/types/type.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/types/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/classes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/codec/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/codec/per/
--rw-rw-rw-   0        0        0    52439 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/codec/per/decoder.py
--rw-rw-rw-   0        0        0    40151 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/codec/per/encoder.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/codec/per/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/codec/__init__.py
--rw-rw-rw-   0        0        0      703 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/logging.cfg
--rw-rw-rw-   0        0        0      234 2023-03-24 10:06:58.000000 asn1PERser-0.4.2/asn1PERser/logging_setup.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/dict_creation/
--rw-rw-rw-   0        0        0    11099 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/test/dict_creation/test_to_dict.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/dict_creation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/
--rw-rw-rw-   0        0        0     1090 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Choice_Simple.py
--rw-rw-rw-   0        0        0     1261 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes.py
--rw-rw-rw-   0        0        0     5009 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_containing_ComponentTypes.py
--rw-rw-rw-   0        0        0     2494 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAddition.py
--rw-rw-rw-   0        0        0     2710 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAdditionGroup.py
--rw-rw-rw-   0        0        0     1794 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionMarker.py
--rw-rw-rw-   0        0        0     1997 2023-03-24 12:32:04.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/DefinedType_Simple.py
--rw-rw-rw-   0        0        0     2721 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Default.py
--rw-rw-rw-   0        0        0     2050 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Mixed.py
--rw-rw-rw-   0        0        0     1557 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Simple.py
--rw-rw-rw-   0        0        0     2905 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/SimpleProtocol.py
--rw-rw-rw-   0        0        0     2236 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/SimpleTypes.py
--rw-rw-rw-   0        0        0     1713 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Types_constrained.py
--rw-rw-rw-   0        0        0     3048 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Types_containing_constrained_types.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/__init__.py
--rw-rw-rw-   0        0        0      870 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/conftest.py
--rw-rw-rw-   0        0        0     1198 2023-03-24 08:47:18.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/test_parse_simple_schemas.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/parsing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/per/
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/
--rw-rw-rw-   0        0        0    13917 2023-03-15 23:54:05.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_bitstring.py
--rw-rw-rw-   0        0        0      467 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_boolean.py
--rw-rw-rw-   0        0        0    12010 2023-03-16 11:27:36.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_choice.py
--rw-rw-rw-   0        0        0    16368 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_enumerated.py
--rw-rw-rw-   0        0        0    37970 2023-03-15 13:43:54.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_integer.py
--rw-rw-rw-   0        0        0     2699 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_mixed_schemas.py
--rw-rw-rw-   0        0        0    15813 2023-03-16 00:28:13.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_octetstring.py
--rw-rw-rw-   0        0        0    22313 2023-03-16 09:21:29.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_sequence.py
--rw-rw-rw-   0        0        0     8573 2023-03-20 10:27:14.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_sequence_of.py
--rw-rw-rw-   0        0        0     1000 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_SimpleProtocol.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/decoder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/
--rw-rw-rw-   0        0        0    10752 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_bitstring.py
--rw-rw-rw-   0        0        0      400 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_boolean.py
--rw-rw-rw-   0        0        0    17078 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_choice.py
--rw-rw-rw-   0        0        0    13137 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_enumerated.py
--rw-rw-rw-   0        0        0    36904 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_integer.py
--rw-rw-rw-   0        0        0     8678 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_mixed_schemas.py
--rw-rw-rw-   0        0        0    11677 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_octetstring.py
--rw-rw-rw-   0        0        0    38898 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_sequence.py
--rw-rw-rw-   0        0        0    10153 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_sequence_of.py
--rw-rw-rw-   0        0        0     3794 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_SimpleProtocol.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/encoder/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/per/__init__.py
--rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/asn1PERser/test/__init__.py
--rw-rw-rw-   0        0        0      597 2023-03-24 10:06:58.000000 asn1PERser-0.4.2/asn1PERser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    20716 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       61 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/requires.txt
--rw-rw-rw-   0        0        0     5557 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/asn1PERser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2021-05-12 06:49:30.000000 asn1PERser-0.4.2/LICENSE
--rw-rw-rw-   0        0        0    20716 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    15331 2023-03-28 08:41:28.000000 asn1PERser-0.4.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-29 13:22:44.000000 asn1PERser-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1125 2023-03-29 13:17:03.000000 asn1PERser-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/
+-rw-rw-rw-   0        0        0     1086 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0    16491 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15821 2023-07-14 08:27:30.000000 asn1PERser-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/
+-rw-rw-rw-   0        0        0      619 2023-07-14 08:14:46.000000 asn1PERser-0.4.3/asn1PERser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/__init__.py
+-rw-rw-rw-   0        0        0      435 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/assignment_def.py
+-rw-rw-rw-   0        0        0     4006 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/character_and_word_set.py
+-rw-rw-rw-   0        0        0     1693 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/common_def.py
+-rw-rw-rw-   0        0        0     3735 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/constraint_def.py
+-rw-rw-rw-   0        0        0     4475 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/lexical_items.py
+-rw-rw-rw-   0        0        0     4238 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/module_def.py
+-rw-rw-rw-   0        0        0    11036 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/type_def.py
+-rw-rw-rw-   0        0        0     2524 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/asn_definitions/value_def.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/data/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/
+-rw-rw-rw-   0        0        0      683 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/BitStringType.py
+-rw-rw-rw-   0        0        0      552 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/BooleanType.py
+-rw-rw-rw-   0        0        0     1044 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/ChoiceType.py
+-rw-rw-rw-   0        0        0      737 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/EnumeratedType.py
+-rw-rw-rw-   0        0        0      799 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/IntegerType.py
+-rw-rw-rw-   0        0        0      737 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/OctetStringType.py
+-rw-rw-rw-   0        0        0     1199 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/SequenceOfType.py
+-rw-rw-rw-   0        0        0     1699 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/SequenceType.py
+-rw-rw-rw-   0        0        0       86 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/UTF8String.py
+-rw-rw-rw-   0        0        0      364 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/data/builtin/__init__.py
+-rw-rw-rw-   0        0        0     8636 2023-07-13 10:48:02.000000 asn1PERser-0.4.3/asn1PERser/classes/module.py
+-rw-rw-rw-   0        0        0     5199 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/parse_actions.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/
+-rw-rw-rw-   0        0        0      471 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/__init__.py
+-rw-rw-rw-   0        0        0      704 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/creator.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/
+-rw-rw-rw-   0        0        0      457 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/BitStringType.txt
+-rw-rw-rw-   0        0        0       59 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/BooleanType.txt
+-rw-rw-rw-   0        0        0     1898 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/ChoiceType.txt
+-rw-rw-rw-   0        0        0       43 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/DefinedType.txt
+-rw-rw-rw-   0        0        0      697 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/EnumeratedType.txt
+-rw-rw-rw-   0        0        0      459 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/IntegerType.txt
+-rw-rw-rw-   0        0        0      457 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/OctetStringType.txt
+-rw-rw-rw-   0        0        0      507 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/SequenceOfType.txt
+-rw-rw-rw-   0        0        0     3015 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/SequenceType.txt
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/__init__.py
+-rw-rw-rw-   0        0        0      439 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/header.txt
+-rw-rw-rw-   0        0        0       60 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/simple_value.txt
+-rw-rw-rw-   0        0        0       46 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/templates/files/type_type.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/types/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/
+-rw-rw-rw-   0        0        0     1673 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/BitStringType.py
+-rw-rw-rw-   0        0        0     1262 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/BooleanType.py
+-rw-rw-rw-   0        0        0     5247 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/ChoiceType.py
+-rw-rw-rw-   0        0        0      156 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/DateType.py
+-rw-rw-rw-   0        0        0     2029 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/DefinedType.py
+-rw-rw-rw-   0        0        0     2569 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/EnumeratedType.py
+-rw-rw-rw-   0        0        0      175 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/IA5String.py
+-rw-rw-rw-   0        0        0     1460 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/IntegerType.py
+-rw-rw-rw-   0        0        0      168 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/NullType.py
+-rw-rw-rw-   0        0        0      187 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/NumericString.py
+-rw-rw-rw-   0        0        0     1677 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/OctetStringType.py
+-rw-rw-rw-   0        0        0      168 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/RealType.py
+-rw-rw-rw-   0        0        0     1989 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/SequenceOfType.py
+-rw-rw-rw-   0        0        0     6204 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/SequenceType.py
+-rw-rw-rw-   0        0        0      418 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/UTF8String.py
+-rw-rw-rw-   0        0        0      175 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/VisibleString.py
+-rw-rw-rw-   0        0        0      903 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/builtin/__init__.py
+-rw-rw-rw-   0        0        0     4370 2023-03-06 10:13:30.000000 asn1PERser-0.4.3/asn1PERser/classes/types/constraint.py
+-rw-rw-rw-   0        0        0     3553 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/classes/types/type.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/codec/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/codec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/codec/per/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/codec/per/__init__.py
+-rw-rw-rw-   0        0        0    52390 2023-07-13 10:53:45.000000 asn1PERser-0.4.3/asn1PERser/codec/per/decoder.py
+-rw-rw-rw-   0        0        0    40151 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/codec/per/encoder.py
+-rw-rw-rw-   0        0        0      512 2023-07-14 08:34:45.000000 asn1PERser-0.4.3/asn1PERser/logging_setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/dict_creation/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/dict_creation/__init__.py
+-rw-rw-rw-   0        0        0    11099 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/test/dict_creation/test_to_dict.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/
+-rw-rw-rw-   0        0        0     1090 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Choice_Simple.py
+-rw-rw-rw-   0        0        0     1261 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes.py
+-rw-rw-rw-   0        0        0     5009 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_containing_ComponentTypes.py
+-rw-rw-rw-   0        0        0     2494 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAddition.py
+-rw-rw-rw-   0        0        0     2710 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAdditionGroup.py
+-rw-rw-rw-   0        0        0     1794 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionMarker.py
+-rw-rw-rw-   0        0        0     1997 2023-03-24 12:32:04.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/DefinedType_Simple.py
+-rw-rw-rw-   0        0        0     2721 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Default.py
+-rw-rw-rw-   0        0        0     2050 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Mixed.py
+-rw-rw-rw-   0        0        0     1557 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Simple.py
+-rw-rw-rw-   0        0        0     2905 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/SimpleProtocol.py
+-rw-rw-rw-   0        0        0     2236 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/SimpleTypes.py
+-rw-rw-rw-   0        0        0     1713 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Types_constrained.py
+-rw-rw-rw-   0        0        0     3048 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Types_containing_constrained_types.py
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/__init__.py
+-rw-rw-rw-   0        0        0      870 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/conftest.py
+-rw-rw-rw-   0        0        0     1198 2023-03-24 08:47:18.000000 asn1PERser-0.4.3/asn1PERser/test/parsing/test_parse_simple_schemas.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/per/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/__init__.py
+-rw-rw-rw-   0        0        0     1000 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_SimpleProtocol.py
+-rw-rw-rw-   0        0        0    13917 2023-03-15 23:54:05.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_bitstring.py
+-rw-rw-rw-   0        0        0      467 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_boolean.py
+-rw-rw-rw-   0        0        0    12010 2023-03-16 11:27:36.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_choice.py
+-rw-rw-rw-   0        0        0    16368 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_enumerated.py
+-rw-rw-rw-   0        0        0    37970 2023-03-15 13:43:54.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_integer.py
+-rw-rw-rw-   0        0        0     2699 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_mixed_schemas.py
+-rw-rw-rw-   0        0        0    15813 2023-03-16 00:28:13.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_octetstring.py
+-rw-rw-rw-   0        0        0    22313 2023-03-16 09:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_sequence.py
+-rw-rw-rw-   0        0        0     8573 2023-03-20 10:27:14.000000 asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_sequence_of.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/
+-rw-rw-rw-   0        0        0        0 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3794 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_SimpleProtocol.py
+-rw-rw-rw-   0        0        0    10752 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_bitstring.py
+-rw-rw-rw-   0        0        0      400 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_boolean.py
+-rw-rw-rw-   0        0        0    17078 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_choice.py
+-rw-rw-rw-   0        0        0    13137 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_enumerated.py
+-rw-rw-rw-   0        0        0    36904 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_integer.py
+-rw-rw-rw-   0        0        0     8678 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_mixed_schemas.py
+-rw-rw-rw-   0        0        0    11677 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_octetstring.py
+-rw-rw-rw-   0        0        0    38898 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_sequence.py
+-rw-rw-rw-   0        0        0    10153 2021-05-12 06:49:30.000000 asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_sequence_of.py
+drwxrwxrwx   0        0        0        0 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/
+-rw-rw-rw-   0        0        0    16491 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5534 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/asn1PERser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 12:21:29.000000 asn1PERser-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2023-07-13 12:09:04.000000 asn1PERser-0.4.3/setup.py
```

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/character_and_word_set.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/character_and_word_set.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/common_def.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/common_def.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/constraint_def.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/constraint_def.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/lexical_items.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/lexical_items.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/module_def.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/module_def.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/type_def.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/type_def.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/asn_definitions/value_def.py` & `asn1PERser-0.4.3/asn1PERser/asn_definitions/value_def.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/BitStringType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/BitStringType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/BooleanType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/BooleanType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/ChoiceType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/ChoiceType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/EnumeratedType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/EnumeratedType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/IntegerType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/IntegerType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/OctetStringType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/OctetStringType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/SequenceOfType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/SequenceOfType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/data/builtin/SequenceType.py` & `asn1PERser-0.4.3/asn1PERser/classes/data/builtin/SequenceType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/module.py` & `asn1PERser-0.4.3/asn1PERser/classes/module.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/parse_actions.py` & `asn1PERser-0.4.3/asn1PERser/classes/parse_actions.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/templates/creator.py` & `asn1PERser-0.4.3/asn1PERser/classes/templates/creator.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/templates/files/ChoiceType.txt` & `asn1PERser-0.4.3/asn1PERser/classes/templates/files/ChoiceType.txt`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/templates/files/EnumeratedType.txt` & `asn1PERser-0.4.3/asn1PERser/classes/templates/files/EnumeratedType.txt`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/templates/files/SequenceType.txt` & `asn1PERser-0.4.3/asn1PERser/classes/templates/files/SequenceType.txt`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/BitStringType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/BitStringType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/BooleanType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/BooleanType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/ChoiceType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/ChoiceType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/DefinedType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/DefinedType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/EnumeratedType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/EnumeratedType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/IntegerType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/IntegerType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/OctetStringType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/OctetStringType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/SequenceOfType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/SequenceOfType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/SequenceType.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/SequenceType.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/builtin/__init__.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/builtin/__init__.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/constraint.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/constraint.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/classes/types/type.py` & `asn1PERser-0.4.3/asn1PERser/classes/types/type.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/codec/per/decoder.py` & `asn1PERser-0.4.3/asn1PERser/codec/per/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,15 @@
             return '0'
         return self.binary_string[bits_start:bits_stop]
 
     def __len__(self):
         return int(len(self.binary_string) / 8)
 
 
-def decode(per_stream, asn1Spec, log_level=logging.WARNING):
-    logger.setLevel(log_level)
+def decode(per_stream, asn1Spec, **kwargs):
     per_bytes = PerBytes(binascii.hexlify(per_stream))
     logger.debug("Decoding of bytes: '%s' started. Binary representation: '%s'", codecs.encode(per_stream, "hex_codec"), per_bytes.binary_string)
     decoded = asn1Spec.create_field_list(per_bytes)
     if decoded == '':
         return asn1Spec.__class__('')
     return decoded
```

### Comparing `asn1PERser-0.4.2/asn1PERser/codec/per/encoder.py` & `asn1PERser-0.4.3/asn1PERser/codec/per/encoder.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/dict_creation/test_to_dict.py` & `asn1PERser-0.4.3/asn1PERser/test/dict_creation/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Choice_Simple.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Choice_Simple.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_containing_ComponentTypes.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_containing_ComponentTypes.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAddition.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAddition.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAdditionGroup.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionAdditionGroup.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionMarker.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/ComponentTypes_extensionMarker.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/DefinedType_Simple.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/DefinedType_Simple.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Default.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Default.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Mixed.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Mixed.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Sequence_Simple.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Sequence_Simple.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/SimpleProtocol.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/SimpleProtocol.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/SimpleTypes.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/SimpleTypes.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Types_constrained.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Types_constrained.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/asn1_python_code/Types_containing_constrained_types.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/asn1_python_code/Types_containing_constrained_types.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/conftest.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/conftest.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/parsing/test_parse_simple_schemas.py` & `asn1PERser-0.4.3/asn1PERser/test/parsing/test_parse_simple_schemas.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_bitstring.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_bitstring.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_choice.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_choice.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_enumerated.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_enumerated.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_integer.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_integer.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_mixed_schemas.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_mixed_schemas.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_octetstring.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_octetstring.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_sequence.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_sequence.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_sequence_of.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_sequence_of.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/decoder/test_per_decode_SimpleProtocol.py` & `asn1PERser-0.4.3/asn1PERser/test/per/decoder/test_per_decode_SimpleProtocol.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_bitstring.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_bitstring.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_choice.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_choice.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_enumerated.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_enumerated.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_integer.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_integer.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_mixed_schemas.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_mixed_schemas.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_octetstring.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_octetstring.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_sequence.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_sequence.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_sequence_of.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_sequence_of.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/test/per/encoder/test_per_encode_SimpleProtocol.py` & `asn1PERser-0.4.3/asn1PERser/test/per/encoder/test_per_encode_SimpleProtocol.py`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/asn1PERser/__init__.py` & `asn1PERser-0.4.3/asn1PERser/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from asn1PERser.codec.per.decoder import decode
 from asn1PERser.codec.per.encoder import encode
 from asn1PERser.classes.module import remove_comments
 from asn1PERser.asn_definitions.module_def import ModuleDefinition
-from asn1PERser.logging_setup import logging_setup
+from asn1PERser.logging_setup import asn1perser_logging_setup
 
 
 __all__ = ['decode', 'encode', 'parse_asn1_schema']
 
-logging_setup()
+asn1perser_logging_setup()
 
 def parse_asn1_schema(asn1_schema, output_folder=None):
     no_comment_schema = remove_comments(asn1_schema)
     parsed_asn = ModuleDefinition.parseString(no_comment_schema)[0]
     return parsed_asn.create_python_template(path=output_folder)
```

### Comparing `asn1PERser-0.4.2/asn1PERser.egg-info/PKG-INFO` & `asn1PERser-0.4.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,604 +1,600 @@
-Metadata-Version: 2.1
-Name: asn1PERser
-Version: 0.4.2
-Summary: Parse ASN.1 schemas into Python code and encode/decode them using PER encoder
-Home-page: https://github.com/erupikus/asn1PERser
-Author: Maciej Pikuła
-Author-email: erupikus@gmail.com
-License: UNKNOWN
-Description: # asn1PERser
-        This library can parse ASN.1 text schemas into Python code. ASN.1 PER (Aligned) decoder/encoder is included to use with parsed schemas.
-        
-        Supported ASN.1 types and their constraints are:
-        
-        | ASN.1 Type   | Single value | Value range | Value size | can be extended (...) | used Python contraint class |
-        |:------------:|:------------:|:-----------:|:----------:|:---------------------:|:---------------------------:|
-        | INTEGER      |      X       |     X       |            |       X               |       ValueRange            |
-        | BOOLEAN      |              |             |            |                       |                             |
-        | ENUMERATED   |              |             |            |       X               |       ExtensionMarker       |
-        | BIT STRING   |      X       |             |     X      |       X               |       ValueSize             |
-        | OCTET STRING |      X       |             |     X      |       X               |       ValueSize             |
-        | CHOICE       |              |             |            |       X               |       ExtensionMarker       |
-        | SEQUENCE     |              |             |            |       X               |       ExtensionMarker       |
-        | SEQUENCE OF  |      X       |             |     X      |       X               |       SequenceOfValueSize   |
-        
-        Table of contents:
-        1. [Examples](#examples)
-        2. [Decoding from string](#decoding-from-string)
-        3. [Dictionary creation](#dictionary-creation)
-        4. [Additional info](#additional-info)
-        5. [History](#history)
-        6. [Known bugs](#known-bugs)
-        
-        ## Examples
-        Following ASN.1 schema:
-        
-        ```python
-        asn_schema = '''\
-        SimpleProtocol DEFINITIONS AUTOMATIC TAGS ::=
-        BEGIN
-        SimpleMessage ::= CHOICE {
-            start    Start,
-            stop     Stop,
-            alive    Alive,
-            data     Data,
-            ...
-        }
-        
-        Start ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            timestamp         UTC-Timestamp,
-            srcPort           Port,
-            dstPort           Port
-        }
-        
-        Stop ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            timestamp         UTC-Timestamp,
-            srcPort           Port,
-            dstPort           Port
-        }
-        
-        Alive ::= SEQUENCE {
-            timestamp         UTC-Timestamp,
-            ...
-        }
-        
-        Data ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            swRelease         ENUMERATED {rel1, rel2, rel3, ...},
-            macroId           BIT STRING (SIZE(20)) OPTIONAL,
-            payload           Payload
-        }
-        
-        Port ::= INTEGER (10000..65535)
-        
-        SequenceNumber ::= INTEGER (0..65535)
-        
-        UTC-Timestamp ::= SEQUENCE {
-            seconds     INTEGER (0..4294967295),
-            useconds    INTEGER (0..4294967295)
-        }
-        
-        Payload ::= SEQUENCE (SIZE(1..5)) OF Message
-        
-        Message ::= OCTET STRING (SIZE(1..4))
-        
-        END
-        '''
-        ```
-        
-        can be parsed into Python code like this:
-        ```python
-        from asn1PERser import parse_asn1_schema
-        
-        
-        parse_asn1_schema(asn1_schema=asn_schema, output_folder=r'C:/my_code/')
-        ```
-        
-        Above code will create file 'SimpleProtocol.py' in folder (which must exist) 'C:/my_code/':
-        ```python
-        from pyasn1.type.namedtype import NamedType, NamedTypes, OptionalNamedType, DefaultedNamedType
-        from pyasn1.type.namedval import NamedValues
-        from asn1PERser.classes.data.builtin import *
-        from asn1PERser.classes.types.type import AdditiveNamedTypes
-        from asn1PERser.classes.types.constraint import MIN, MAX, NoConstraint, ExtensionMarker, SequenceOfValueSize, \
-            ValueRange, SingleValue, ValueSize, ConstraintOr, ConstraintAnd
-        
-        
-        class Port(IntegerType):
-            subtypeSpec = ValueRange(10000, 65535)
-        
-        
-        class SequenceNumber(IntegerType):
-            subtypeSpec = ValueRange(0, 65535)
-        
-        
-        class Message(OctetStringType):
-            subtypeSpec = ValueSize(1, 4)
-        
-        
-        class UTC_Timestamp(SequenceType):
-            class seconds(IntegerType):
-                subtypeSpec = ValueRange(0, 4294967295)
-        
-            class useconds(IntegerType):
-                subtypeSpec = ValueRange(0, 4294967295)
-        
-            rootComponent = AdditiveNamedTypes(
-                NamedType('seconds', seconds()),
-                NamedType('useconds', useconds()),
-            )
-            componentType = rootComponent
-        
-        
-        class Start(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('timestamp', UTC_Timestamp()),
-                NamedType('srcPort', Port()),
-                NamedType('dstPort', Port()),
-            )
-            componentType = rootComponent
-        
-        
-        class Stop(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('timestamp', UTC_Timestamp()),
-                NamedType('srcPort', Port()),
-                NamedType('dstPort', Port()),
-            )
-            componentType = rootComponent
-        
-        
-        class Alive(SequenceType):
-            subtypeSpec = ExtensionMarker(True)
-            rootComponent = AdditiveNamedTypes(
-                NamedType('timestamp', UTC_Timestamp()),
-            )
-            componentType = rootComponent
-        
-        
-        class Payload(SequenceOfType):
-            subtypeSpec = SequenceOfValueSize(1, 5)
-            componentType = Message()
-        
-        
-        class Data(SequenceType):
-            class swRelease(EnumeratedType):
-                subtypeSpec = ExtensionMarker(True)
-                enumerationRoot = NamedValues(
-                    ('rel1', 0),
-                    ('rel2', 1),
-                    ('rel3', 2),
-                )
-                namedValues = enumerationRoot
-        
-            class macroId(BitStringType):
-                subtypeSpec = ValueSize(20, 20)
-        
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('swRelease', swRelease()),
-                OptionalNamedType('macroId', macroId()),
-                NamedType('payload', Payload()),
-            )
-            componentType = rootComponent
-        
-        
-        class SimpleMessage(ChoiceType):
-            subtypeSpec = ExtensionMarker(True)
-            rootComponent = AdditiveNamedTypes(
-                NamedType('start', Start()),
-                NamedType('stop', Stop()),
-                NamedType('alive', Alive()),
-                NamedType('data', Data()),
-            )
-            componentType = rootComponent
-        
-        
-        
-        ```
-        
-        When schema is parsed it can be used - message can be created, encoded and decoded, using PER encoder/decoder, into bytes
-        or Python structure:
-        ```python
-        from asn1PERser import encode, decode
-        from SimpleProtocol import *
-        
-        
-        '''
-        simple_message SimpleMessage ::= alive : {
-            timestamp {
-                seconds 1557528149,
-                useconds 12345
-            }
-        }
-        '''
-        utc_timestamp = UTC_Timestamp()
-        utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
-        utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
-        
-        msg_alive = Alive()
-        msg_alive['timestamp'] = utc_timestamp
-        
-        simple_message = SimpleMessage()
-        simple_message['alive'] = msg_alive
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded alive bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('decoded alive message structure as string...:')
-        print(decoded)
-        
-        print('...can be accessed like dictionary:')
-        print(decoded['alive']['timestamp']['seconds'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded alive bytes as hex string:
-        4c5cd5fe55403039
-        
-        
-        decoded alive message structure as string...:
-        SimpleMessage:
-         alive=Alive:
-          timestamp=UTC_Timestamp:
-           seconds=1557528149
-           useconds=12345
-        
-        
-        
-        ...can be accessed like dictionary:
-        1557528149
-        
-        
-        ...can be transformed into dictionary:
-        {'alive': OrderedDict([('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)]))])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= start : {
-            sequenceNumber    10,
-            timestamp {
-                seconds 1557528149,
-                useconds 12345
-            },
-            srcPort    65533,
-            dstPort    10000
-        }
-        '''
-        
-        utc_timestamp = UTC_Timestamp()
-        utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
-        utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
-        
-        msg_start = Start()
-        msg_start['sequenceNumber'] = SequenceNumber(10)
-        msg_start['timestamp'] = utc_timestamp
-        msg_start['srcPort'] = Port(65533)
-        msg_start['dstPort'] = Port(10000)
-        
-        simple_message = SimpleMessage()
-        simple_message['start'] = msg_start
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded start bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('start message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(decoded['start']['srcPort'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded start bytes as hex string:
-        00000ac05cd5fe55403039d8ed0000
-        
-        
-        start message structure as string...:
-        SimpleMessage:
-         start=Start:
-          sequenceNumber=10
-          timestamp=UTC_Timestamp:
-           seconds=1557528149
-           useconds=12345
-        
-          srcPort=65533
-          dstPort=10000
-        
-        
-        ...can be accessed like dictionary:
-        65533
-        
-        
-        ...can be transformed into dictionary:
-        {'start': OrderedDict([('sequenceNumber', 10), ('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)])), ('srcPort', 65533), ('dstPort', 10000)])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= data : {
-            sequenceNumber    55555,
-            swRelease  rel2,
-            macroId    '11110000111100001111'B,
-            payload {
-                'DEAD'H,
-                'BEEF'H,
-                'FEED'H,
-                'AA'H,
-                'BBBBBBBB'H
-            }
-        }
-        '''
-        
-        data_payload = Payload()
-        data_payload.extend([Message(hexValue='DEAD')])
-        data_payload.extend([Message(hexValue='BEEF')])
-        data_payload.extend([Message(hexValue='FEED')])
-        data_payload.extend([Message(hexValue='AA')])
-        data_payload.extend([Message(hexValue='BBBBBBBB')])
-        
-        msg_data = Data()
-        msg_data['sequenceNumber'] = SequenceNumber(55555)
-        msg_data['swRelease'] = Data.swRelease('rel2')
-        msg_data['macroId'] = Data.macroId(binValue='11110000111100001111')
-        msg_data['payload'] = data_payload
-        
-        simple_message = SimpleMessage()
-        simple_message['data'] = msg_data
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded data bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('data message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(bytes(decoded['data']['payload'][0]).hex())
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded data bytes as hex string:
-        70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb
-        
-        
-        data message structure as string...:
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=55555
-          swRelease=rel2
-          macroId=986895
-          payload=Payload:
-           0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
-        
-        
-        ...can be accessed like dictionary:
-        dead
-        
-        
-        ...can be transformed into dictionary:
-        {'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= data : {
-            sequenceNumber    256,
-            swRelease  rel3,
-            payload {
-                'DEADBEEF'H
-            }
-        }
-        '''
-        data_payload = Payload()
-        data_payload.extend([Message(hexValue='DEADBEEF')])
-        
-        msg_data = Data()
-        msg_data['sequenceNumber'] = SequenceNumber(256)
-        msg_data['swRelease'] = Data.swRelease('rel3')
-        msg_data['payload'] = data_payload
-        
-        simple_message = SimpleMessage()
-        simple_message['data'] = msg_data
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded data bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('data message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(decoded['data']['swRelease'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded data bytes as hex string:
-        60010043deadbeef
-        
-        
-        data message structure as string...:
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=256
-          swRelease=rel3
-          payload=Payload:
-           0xdeadbeef
-        
-        
-        ...can be accessed like dictionary:
-        rel3
-        
-        
-        ...can be transformed into dictionary:
-        {'data': OrderedDict([('sequenceNumber', 256), ('swRelease', 'rel3'), ('payload', ['deadbeef'])])}
-        ```
-        
-        ## Decoding from string
-        When encoded bytes are given as __string__ use _bytearray.fromhex()_:
-        
-        ```
-        
-        pure_string = str('70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb')
-        real_bytes = bytearray.fromhex(pure_string)
-        
-        decoded = decode(asn1Spec=SimpleMessage(), per_stream=real_bytes)
-        print(decoded)
-        ```
-        
-        above will output:
-        ```
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=55555
-          swRelease=rel2
-          macroId=986895
-          payload=Payload:
-           0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
-        ```
-        
-        ## Dictionary creation
-          Data above can be accessed like dictionary but it is not a dictionary.
-          Method '__to_dict__' was added to make dictionary creation simple:
-        
-        ```
-        msg_dict = decoded.to_dict()
-        print(type(msg_dict))
-        print(msg_dict)
-        ```
-        
-        output:
-        ```
-        <class 'dict'>
-        {'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
-        ```
-        
-        To better show created structure, json.dumps() can be used:
-        ```
-        print(json.dumps(msg_dict, indent=2))
-        ```
-        
-        output:
-        ```
-        {
-          "data": {
-            "sequenceNumber": 55555,
-            "swRelease": "rel2",
-            "macroId": 986895,
-            "payload": [
-              "dead",
-              "beef",
-              "feed",
-              "aa",
-              "bbbbbbbb"
-            ]
-          }
-        }
-        ```
-        
-        ## Additional info
-        
-        For more examples please see library tests:
-        - parsing tests, located in test/parsing/ folder.
-        - coding/encoding tests, located in test/per folder.
-        
-        All above examples and tests where checked using:
-        https://asn1.io/asn1playground/
-        
-        This library inherits extensively from pyasn1 library so BER and other encoding should also work here.
-        
-        Parsing may take time - when trying to parse about 2000 lines of ASN.1 it took 15-20 minutes.
-        Tests for parsing also take time.
-        
-        ## History
-        
-        See CHANGES file.
-        
-        ## Known bugs
-        - Defining BitStringType type with default hexValue set to empty string (''), like:
-        ```
-        ...
-        d15     BIT STRING DEFAULT ''H,
-        ...
-        ```
-        will parse to Python code but running it will cause exception:
-        ```
-        pyasn1.error.PyAsn1Error: BitStringType.fromHexString() error: invalid literal for int() with base 16: ''
-        ```
-        
-        - This will parse, but sorting algorith may not sort it corretly:
-        ```
-            
-            MySeq2 ::= MySeq1   -- ok since one level of nesting is ok
-        
-            MySeq3 ::= MySeq1   -- ok since one level of nesting is ok
-            
-            MySeq1 ::= SEQUENCE {
-                d00     INTEGER
-            }
-        
-            MySeq4 ::= MySeq2   -- NOT OK! 2nd level of nesting 
-        ```
-        This will parse into:
-        ```python
-        MySeq4 = MySeq2
-        
-        
-        class MySeq1(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('d00', IntegerType()),
-            )
-            componentType = rootComponent
-        
-        
-        MySeq3 = MySeq1
-        
-        
-        MySeq2 = MySeq1
-        ```
-        so Python will not find MySeq2 - this will lead to NameError.
-        
-Keywords: asn asn1 asn.1 PER decoder encoder
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# asn1PERser
+This library can parse ASN.1 text schemas into Python code. ASN.1 PER (Aligned) decoder/encoder is included to use with parsed schemas.
+
+Supported ASN.1 types and their constraints are:
+
+| ASN.1 Type   | Single value | Value range | Value size | can be extended (...) | used Python contraint class |
+|:------------:|:------------:|:-----------:|:----------:|:---------------------:|:---------------------------:|
+| INTEGER      |      X       |     X       |            |       X               |       ValueRange            |
+| BOOLEAN      |              |             |            |                       |                             |
+| ENUMERATED   |              |             |            |       X               |       ExtensionMarker       |
+| BIT STRING   |      X       |             |     X      |       X               |       ValueSize             |
+| OCTET STRING |      X       |             |     X      |       X               |       ValueSize             |
+| CHOICE       |              |             |            |       X               |       ExtensionMarker       |
+| SEQUENCE     |              |             |            |       X               |       ExtensionMarker       |
+| SEQUENCE OF  |      X       |             |     X      |       X               |       SequenceOfValueSize   |
+
+Table of contents:
+1. [Examples](#examples)
+2. [Decoding from string](#decoding-from-string)
+3. [Dictionary creation](#dictionary-creation)
+4. [Additional info](#additional-info)
+5. [History](#history)
+6. [Known bugs](#known-bugs)
+
+## Examples
+Following ASN.1 schema:
+
+```python
+asn_schema = '''\
+SimpleProtocol DEFINITIONS AUTOMATIC TAGS ::=
+BEGIN
+SimpleMessage ::= CHOICE {
+    start    Start,
+    stop     Stop,
+    alive    Alive,
+    data     Data,
+    ...
+}
+
+Start ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    timestamp         UTC-Timestamp,
+    srcPort           Port,
+    dstPort           Port
+}
+
+Stop ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    timestamp         UTC-Timestamp,
+    srcPort           Port,
+    dstPort           Port
+}
+
+Alive ::= SEQUENCE {
+    timestamp         UTC-Timestamp,
+    ...
+}
+
+Data ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    swRelease         ENUMERATED {rel1, rel2, rel3, ...},
+    macroId           BIT STRING (SIZE(20)) OPTIONAL,
+    payload           Payload
+}
+
+Port ::= INTEGER (10000..65535)
+
+SequenceNumber ::= INTEGER (0..65535)
+
+UTC-Timestamp ::= SEQUENCE {
+    seconds     INTEGER (0..4294967295),
+    useconds    INTEGER (0..4294967295)
+}
+
+Payload ::= SEQUENCE (SIZE(1..5)) OF Message
+
+Message ::= OCTET STRING (SIZE(1..4))
+
+END
+'''
+```
+
+can be parsed into Python code like this:
+```python
+from asn1PERser import parse_asn1_schema
+
+
+parse_asn1_schema(asn1_schema=asn_schema, output_folder=r'C:/my_code/')
+```
+
+Above code will create file 'SimpleProtocol.py' in folder (which must exist) 'C:/my_code/':
+```python
+from pyasn1.type.namedtype import NamedType, NamedTypes, OptionalNamedType, DefaultedNamedType
+from pyasn1.type.namedval import NamedValues
+from asn1PERser.classes.data.builtin import *
+from asn1PERser.classes.types.type import AdditiveNamedTypes
+from asn1PERser.classes.types.constraint import MIN, MAX, NoConstraint, ExtensionMarker, SequenceOfValueSize, \
+    ValueRange, SingleValue, ValueSize, ConstraintOr, ConstraintAnd
+
+
+class Port(IntegerType):
+    subtypeSpec = ValueRange(10000, 65535)
+
+
+class SequenceNumber(IntegerType):
+    subtypeSpec = ValueRange(0, 65535)
+
+
+class Message(OctetStringType):
+    subtypeSpec = ValueSize(1, 4)
+
+
+class UTC_Timestamp(SequenceType):
+    class seconds(IntegerType):
+        subtypeSpec = ValueRange(0, 4294967295)
+
+    class useconds(IntegerType):
+        subtypeSpec = ValueRange(0, 4294967295)
+
+    rootComponent = AdditiveNamedTypes(
+        NamedType('seconds', seconds()),
+        NamedType('useconds', useconds()),
+    )
+    componentType = rootComponent
+
+
+class Start(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('timestamp', UTC_Timestamp()),
+        NamedType('srcPort', Port()),
+        NamedType('dstPort', Port()),
+    )
+    componentType = rootComponent
+
+
+class Stop(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('timestamp', UTC_Timestamp()),
+        NamedType('srcPort', Port()),
+        NamedType('dstPort', Port()),
+    )
+    componentType = rootComponent
+
+
+class Alive(SequenceType):
+    subtypeSpec = ExtensionMarker(True)
+    rootComponent = AdditiveNamedTypes(
+        NamedType('timestamp', UTC_Timestamp()),
+    )
+    componentType = rootComponent
+
+
+class Payload(SequenceOfType):
+    subtypeSpec = SequenceOfValueSize(1, 5)
+    componentType = Message()
+
+
+class Data(SequenceType):
+    class swRelease(EnumeratedType):
+        subtypeSpec = ExtensionMarker(True)
+        enumerationRoot = NamedValues(
+            ('rel1', 0),
+            ('rel2', 1),
+            ('rel3', 2),
+        )
+        namedValues = enumerationRoot
+
+    class macroId(BitStringType):
+        subtypeSpec = ValueSize(20, 20)
+
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('swRelease', swRelease()),
+        OptionalNamedType('macroId', macroId()),
+        NamedType('payload', Payload()),
+    )
+    componentType = rootComponent
+
+
+class SimpleMessage(ChoiceType):
+    subtypeSpec = ExtensionMarker(True)
+    rootComponent = AdditiveNamedTypes(
+        NamedType('start', Start()),
+        NamedType('stop', Stop()),
+        NamedType('alive', Alive()),
+        NamedType('data', Data()),
+    )
+    componentType = rootComponent
+
+
+
+```
+
+When schema is parsed it can be used - message can be created, encoded and decoded, using PER encoder/decoder, into bytes
+or Python structure:
+```python
+from asn1PERser import encode, decode
+from SimpleProtocol import *
+
+
+'''
+simple_message SimpleMessage ::= alive : {
+    timestamp {
+        seconds 1557528149,
+        useconds 12345
+    }
+}
+'''
+utc_timestamp = UTC_Timestamp()
+utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
+utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
+
+msg_alive = Alive()
+msg_alive['timestamp'] = utc_timestamp
+
+simple_message = SimpleMessage()
+simple_message['alive'] = msg_alive
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded alive bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('decoded alive message structure as string...:')
+print(decoded)
+
+print('...can be accessed like dictionary:')
+print(decoded['alive']['timestamp']['seconds'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded alive bytes as hex string:
+4c5cd5fe55403039
+
+
+decoded alive message structure as string...:
+SimpleMessage:
+ alive=Alive:
+  timestamp=UTC_Timestamp:
+   seconds=1557528149
+   useconds=12345
+
+
+
+...can be accessed like dictionary:
+1557528149
+
+
+...can be transformed into dictionary:
+{'alive': OrderedDict([('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)]))])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= start : {
+    sequenceNumber    10,
+    timestamp {
+        seconds 1557528149,
+        useconds 12345
+    },
+    srcPort    65533,
+    dstPort    10000
+}
+'''
+
+utc_timestamp = UTC_Timestamp()
+utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
+utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
+
+msg_start = Start()
+msg_start['sequenceNumber'] = SequenceNumber(10)
+msg_start['timestamp'] = utc_timestamp
+msg_start['srcPort'] = Port(65533)
+msg_start['dstPort'] = Port(10000)
+
+simple_message = SimpleMessage()
+simple_message['start'] = msg_start
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded start bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('start message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(decoded['start']['srcPort'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded start bytes as hex string:
+00000ac05cd5fe55403039d8ed0000
+
+
+start message structure as string...:
+SimpleMessage:
+ start=Start:
+  sequenceNumber=10
+  timestamp=UTC_Timestamp:
+   seconds=1557528149
+   useconds=12345
+
+  srcPort=65533
+  dstPort=10000
+
+
+...can be accessed like dictionary:
+65533
+
+
+...can be transformed into dictionary:
+{'start': OrderedDict([('sequenceNumber', 10), ('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)])), ('srcPort', 65533), ('dstPort', 10000)])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= data : {
+    sequenceNumber    55555,
+    swRelease  rel2,
+    macroId    '11110000111100001111'B,
+    payload {
+        'DEAD'H,
+        'BEEF'H,
+        'FEED'H,
+        'AA'H,
+        'BBBBBBBB'H
+    }
+}
+'''
+
+data_payload = Payload()
+data_payload.extend([Message(hexValue='DEAD')])
+data_payload.extend([Message(hexValue='BEEF')])
+data_payload.extend([Message(hexValue='FEED')])
+data_payload.extend([Message(hexValue='AA')])
+data_payload.extend([Message(hexValue='BBBBBBBB')])
+
+msg_data = Data()
+msg_data['sequenceNumber'] = SequenceNumber(55555)
+msg_data['swRelease'] = Data.swRelease('rel2')
+msg_data['macroId'] = Data.macroId(binValue='11110000111100001111')
+msg_data['payload'] = data_payload
+
+simple_message = SimpleMessage()
+simple_message['data'] = msg_data
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded data bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('data message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(bytes(decoded['data']['payload'][0]).hex())
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded data bytes as hex string:
+70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb
+
+
+data message structure as string...:
+SimpleMessage:
+ data=Data:
+  sequenceNumber=55555
+  swRelease=rel2
+  macroId=986895
+  payload=Payload:
+   0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
+
+
+...can be accessed like dictionary:
+dead
+
+
+...can be transformed into dictionary:
+{'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= data : {
+    sequenceNumber    256,
+    swRelease  rel3,
+    payload {
+        'DEADBEEF'H
+    }
+}
+'''
+data_payload = Payload()
+data_payload.extend([Message(hexValue='DEADBEEF')])
+
+msg_data = Data()
+msg_data['sequenceNumber'] = SequenceNumber(256)
+msg_data['swRelease'] = Data.swRelease('rel3')
+msg_data['payload'] = data_payload
+
+simple_message = SimpleMessage()
+simple_message['data'] = msg_data
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded data bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('data message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(decoded['data']['swRelease'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded data bytes as hex string:
+60010043deadbeef
+
+
+data message structure as string...:
+SimpleMessage:
+ data=Data:
+  sequenceNumber=256
+  swRelease=rel3
+  payload=Payload:
+   0xdeadbeef
+
+
+...can be accessed like dictionary:
+rel3
+
+
+...can be transformed into dictionary:
+{'data': OrderedDict([('sequenceNumber', 256), ('swRelease', 'rel3'), ('payload', ['deadbeef'])])}
+```
+
+## Decoding from string
+When encoded bytes are given as __string__ use _bytearray.fromhex()_:
+
+```
+
+pure_string = str('70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb')
+real_bytes = bytearray.fromhex(pure_string)
+
+decoded = decode(asn1Spec=SimpleMessage(), per_stream=real_bytes)
+print(decoded)
+```
+
+above will output:
+```
+SimpleMessage:
+ data=Data:
+  sequenceNumber=55555
+  swRelease=rel2
+  macroId=986895
+  payload=Payload:
+   0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
+```
+
+## Dictionary creation
+  Data above can be accessed like dictionary but it is not a dictionary.
+  Method '__to_dict__' was added to make dictionary creation simple:
+
+```
+msg_dict = decoded.to_dict()
+print(type(msg_dict))
+print(msg_dict)
+```
+
+output:
+```
+<class 'dict'>
+{'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
+```
+
+To better show created structure, json.dumps() can be used:
+```
+print(json.dumps(msg_dict, indent=2))
+```
+
+output:
+```
+{
+  "data": {
+    "sequenceNumber": 55555,
+    "swRelease": "rel2",
+    "macroId": 986895,
+    "payload": [
+      "dead",
+      "beef",
+      "feed",
+      "aa",
+      "bbbbbbbb"
+    ]
+  }
+}
+```
+
+## Additional info
+
+For more examples please see library tests:
+- parsing tests, located in test/parsing/ folder.
+- coding/encoding tests, located in test/per folder.
+
+All above examples and tests where checked using:
+https://asn1.io/asn1playground/
+
+This library inherits extensively from pyasn1 library so BER and other encoding should also work here.
+
+Parsing may take time - when trying to parse about 2000 lines of ASN.1 it took 15-20 minutes.
+Tests for parsing also take time.
+
+asn1PERser uses logging library (for now only in decoder.py module).
+By default logging.NullHandler() is set as library top handler so no logs are visible.
+If you want to enable logging call asn1perser_logging_setup with (at least) handler
+parameter set to something else than logging.NullHandler:
+
+```
+import logging
+from asn1PERser import asn1perser_logging_setup
+
+asn1perser_logging_setup(logging.StreamHandler())
+```
+
+Above will print logging.INFO level logs to console.
+
+## History
+
+See CHANGES file.
+
+## Known bugs
+- Defining BitStringType type with default hexValue set to empty string (''), like:
+```
+...
+d15     BIT STRING DEFAULT ''H,
+...
+```
+will parse to Python code but running it will cause exception:
+```
+pyasn1.error.PyAsn1Error: BitStringType.fromHexString() error: invalid literal for int() with base 16: ''
+```
+
+- This will parse, but sorting algorith may not sort it corretly:
+```
+    
+    MySeq2 ::= MySeq1   -- ok since one level of nesting is ok
+
+    MySeq3 ::= MySeq1   -- ok since one level of nesting is ok
+    
+    MySeq1 ::= SEQUENCE {
+        d00     INTEGER
+    }
+
+    MySeq4 ::= MySeq2   -- NOT OK! 2nd level of nesting 
+```
+This will parse into:
+```python
+MySeq4 = MySeq2
+
+
+class MySeq1(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('d00', IntegerType()),
+    )
+    componentType = rootComponent
+
+
+MySeq3 = MySeq1
+
+
+MySeq2 = MySeq1
+```
+so Python will not find MySeq2 - this will lead to NameError.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `asn1PERser-0.4.2/asn1PERser.egg-info/SOURCES.txt` & `asn1PERser-0.4.3/asn1PERser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 asn1PERser/__init__.py
-asn1PERser/logging.cfg
 asn1PERser/logging_setup.py
 asn1PERser.egg-info/PKG-INFO
 asn1PERser.egg-info/SOURCES.txt
 asn1PERser.egg-info/dependency_links.txt
 asn1PERser.egg-info/requires.txt
 asn1PERser.egg-info/top_level.txt
 asn1PERser/asn_definitions/__init__.py
```

### Comparing `asn1PERser-0.4.2/LICENSE` & `asn1PERser-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asn1PERser-0.4.2/PKG-INFO` & `asn1PERser-0.4.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,604 +1,617 @@
 Metadata-Version: 2.1
 Name: asn1PERser
-Version: 0.4.2
+Version: 0.4.3
 Summary: Parse ASN.1 schemas into Python code and encode/decode them using PER encoder
 Home-page: https://github.com/erupikus/asn1PERser
 Author: Maciej Pikuła
 Author-email: erupikus@gmail.com
-License: UNKNOWN
-Description: # asn1PERser
-        This library can parse ASN.1 text schemas into Python code. ASN.1 PER (Aligned) decoder/encoder is included to use with parsed schemas.
-        
-        Supported ASN.1 types and their constraints are:
-        
-        | ASN.1 Type   | Single value | Value range | Value size | can be extended (...) | used Python contraint class |
-        |:------------:|:------------:|:-----------:|:----------:|:---------------------:|:---------------------------:|
-        | INTEGER      |      X       |     X       |            |       X               |       ValueRange            |
-        | BOOLEAN      |              |             |            |                       |                             |
-        | ENUMERATED   |              |             |            |       X               |       ExtensionMarker       |
-        | BIT STRING   |      X       |             |     X      |       X               |       ValueSize             |
-        | OCTET STRING |      X       |             |     X      |       X               |       ValueSize             |
-        | CHOICE       |              |             |            |       X               |       ExtensionMarker       |
-        | SEQUENCE     |              |             |            |       X               |       ExtensionMarker       |
-        | SEQUENCE OF  |      X       |             |     X      |       X               |       SequenceOfValueSize   |
-        
-        Table of contents:
-        1. [Examples](#examples)
-        2. [Decoding from string](#decoding-from-string)
-        3. [Dictionary creation](#dictionary-creation)
-        4. [Additional info](#additional-info)
-        5. [History](#history)
-        6. [Known bugs](#known-bugs)
-        
-        ## Examples
-        Following ASN.1 schema:
-        
-        ```python
-        asn_schema = '''\
-        SimpleProtocol DEFINITIONS AUTOMATIC TAGS ::=
-        BEGIN
-        SimpleMessage ::= CHOICE {
-            start    Start,
-            stop     Stop,
-            alive    Alive,
-            data     Data,
-            ...
-        }
-        
-        Start ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            timestamp         UTC-Timestamp,
-            srcPort           Port,
-            dstPort           Port
-        }
-        
-        Stop ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            timestamp         UTC-Timestamp,
-            srcPort           Port,
-            dstPort           Port
-        }
-        
-        Alive ::= SEQUENCE {
-            timestamp         UTC-Timestamp,
-            ...
-        }
-        
-        Data ::= SEQUENCE {
-            sequenceNumber    SequenceNumber,
-            swRelease         ENUMERATED {rel1, rel2, rel3, ...},
-            macroId           BIT STRING (SIZE(20)) OPTIONAL,
-            payload           Payload
-        }
-        
-        Port ::= INTEGER (10000..65535)
-        
-        SequenceNumber ::= INTEGER (0..65535)
-        
-        UTC-Timestamp ::= SEQUENCE {
-            seconds     INTEGER (0..4294967295),
-            useconds    INTEGER (0..4294967295)
-        }
-        
-        Payload ::= SEQUENCE (SIZE(1..5)) OF Message
-        
-        Message ::= OCTET STRING (SIZE(1..4))
-        
-        END
-        '''
-        ```
-        
-        can be parsed into Python code like this:
-        ```python
-        from asn1PERser import parse_asn1_schema
-        
-        
-        parse_asn1_schema(asn1_schema=asn_schema, output_folder=r'C:/my_code/')
-        ```
-        
-        Above code will create file 'SimpleProtocol.py' in folder (which must exist) 'C:/my_code/':
-        ```python
-        from pyasn1.type.namedtype import NamedType, NamedTypes, OptionalNamedType, DefaultedNamedType
-        from pyasn1.type.namedval import NamedValues
-        from asn1PERser.classes.data.builtin import *
-        from asn1PERser.classes.types.type import AdditiveNamedTypes
-        from asn1PERser.classes.types.constraint import MIN, MAX, NoConstraint, ExtensionMarker, SequenceOfValueSize, \
-            ValueRange, SingleValue, ValueSize, ConstraintOr, ConstraintAnd
-        
-        
-        class Port(IntegerType):
-            subtypeSpec = ValueRange(10000, 65535)
-        
-        
-        class SequenceNumber(IntegerType):
-            subtypeSpec = ValueRange(0, 65535)
-        
-        
-        class Message(OctetStringType):
-            subtypeSpec = ValueSize(1, 4)
-        
-        
-        class UTC_Timestamp(SequenceType):
-            class seconds(IntegerType):
-                subtypeSpec = ValueRange(0, 4294967295)
-        
-            class useconds(IntegerType):
-                subtypeSpec = ValueRange(0, 4294967295)
-        
-            rootComponent = AdditiveNamedTypes(
-                NamedType('seconds', seconds()),
-                NamedType('useconds', useconds()),
-            )
-            componentType = rootComponent
-        
-        
-        class Start(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('timestamp', UTC_Timestamp()),
-                NamedType('srcPort', Port()),
-                NamedType('dstPort', Port()),
-            )
-            componentType = rootComponent
-        
-        
-        class Stop(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('timestamp', UTC_Timestamp()),
-                NamedType('srcPort', Port()),
-                NamedType('dstPort', Port()),
-            )
-            componentType = rootComponent
-        
-        
-        class Alive(SequenceType):
-            subtypeSpec = ExtensionMarker(True)
-            rootComponent = AdditiveNamedTypes(
-                NamedType('timestamp', UTC_Timestamp()),
-            )
-            componentType = rootComponent
-        
-        
-        class Payload(SequenceOfType):
-            subtypeSpec = SequenceOfValueSize(1, 5)
-            componentType = Message()
-        
-        
-        class Data(SequenceType):
-            class swRelease(EnumeratedType):
-                subtypeSpec = ExtensionMarker(True)
-                enumerationRoot = NamedValues(
-                    ('rel1', 0),
-                    ('rel2', 1),
-                    ('rel3', 2),
-                )
-                namedValues = enumerationRoot
-        
-            class macroId(BitStringType):
-                subtypeSpec = ValueSize(20, 20)
-        
-            rootComponent = AdditiveNamedTypes(
-                NamedType('sequenceNumber', SequenceNumber()),
-                NamedType('swRelease', swRelease()),
-                OptionalNamedType('macroId', macroId()),
-                NamedType('payload', Payload()),
-            )
-            componentType = rootComponent
-        
-        
-        class SimpleMessage(ChoiceType):
-            subtypeSpec = ExtensionMarker(True)
-            rootComponent = AdditiveNamedTypes(
-                NamedType('start', Start()),
-                NamedType('stop', Stop()),
-                NamedType('alive', Alive()),
-                NamedType('data', Data()),
-            )
-            componentType = rootComponent
-        
-        
-        
-        ```
-        
-        When schema is parsed it can be used - message can be created, encoded and decoded, using PER encoder/decoder, into bytes
-        or Python structure:
-        ```python
-        from asn1PERser import encode, decode
-        from SimpleProtocol import *
-        
-        
-        '''
-        simple_message SimpleMessage ::= alive : {
-            timestamp {
-                seconds 1557528149,
-                useconds 12345
-            }
-        }
-        '''
-        utc_timestamp = UTC_Timestamp()
-        utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
-        utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
-        
-        msg_alive = Alive()
-        msg_alive['timestamp'] = utc_timestamp
-        
-        simple_message = SimpleMessage()
-        simple_message['alive'] = msg_alive
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded alive bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('decoded alive message structure as string...:')
-        print(decoded)
-        
-        print('...can be accessed like dictionary:')
-        print(decoded['alive']['timestamp']['seconds'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded alive bytes as hex string:
-        4c5cd5fe55403039
-        
-        
-        decoded alive message structure as string...:
-        SimpleMessage:
-         alive=Alive:
-          timestamp=UTC_Timestamp:
-           seconds=1557528149
-           useconds=12345
-        
-        
-        
-        ...can be accessed like dictionary:
-        1557528149
-        
-        
-        ...can be transformed into dictionary:
-        {'alive': OrderedDict([('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)]))])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= start : {
-            sequenceNumber    10,
-            timestamp {
-                seconds 1557528149,
-                useconds 12345
-            },
-            srcPort    65533,
-            dstPort    10000
-        }
-        '''
-        
-        utc_timestamp = UTC_Timestamp()
-        utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
-        utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
-        
-        msg_start = Start()
-        msg_start['sequenceNumber'] = SequenceNumber(10)
-        msg_start['timestamp'] = utc_timestamp
-        msg_start['srcPort'] = Port(65533)
-        msg_start['dstPort'] = Port(10000)
-        
-        simple_message = SimpleMessage()
-        simple_message['start'] = msg_start
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded start bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('start message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(decoded['start']['srcPort'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded start bytes as hex string:
-        00000ac05cd5fe55403039d8ed0000
-        
-        
-        start message structure as string...:
-        SimpleMessage:
-         start=Start:
-          sequenceNumber=10
-          timestamp=UTC_Timestamp:
-           seconds=1557528149
-           useconds=12345
-        
-          srcPort=65533
-          dstPort=10000
-        
-        
-        ...can be accessed like dictionary:
-        65533
-        
-        
-        ...can be transformed into dictionary:
-        {'start': OrderedDict([('sequenceNumber', 10), ('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)])), ('srcPort', 65533), ('dstPort', 10000)])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= data : {
-            sequenceNumber    55555,
-            swRelease  rel2,
-            macroId    '11110000111100001111'B,
-            payload {
-                'DEAD'H,
-                'BEEF'H,
-                'FEED'H,
-                'AA'H,
-                'BBBBBBBB'H
-            }
-        }
-        '''
-        
-        data_payload = Payload()
-        data_payload.extend([Message(hexValue='DEAD')])
-        data_payload.extend([Message(hexValue='BEEF')])
-        data_payload.extend([Message(hexValue='FEED')])
-        data_payload.extend([Message(hexValue='AA')])
-        data_payload.extend([Message(hexValue='BBBBBBBB')])
-        
-        msg_data = Data()
-        msg_data['sequenceNumber'] = SequenceNumber(55555)
-        msg_data['swRelease'] = Data.swRelease('rel2')
-        msg_data['macroId'] = Data.macroId(binValue='11110000111100001111')
-        msg_data['payload'] = data_payload
-        
-        simple_message = SimpleMessage()
-        simple_message['data'] = msg_data
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded data bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('data message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(bytes(decoded['data']['payload'][0]).hex())
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded data bytes as hex string:
-        70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb
-        
-        
-        data message structure as string...:
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=55555
-          swRelease=rel2
-          macroId=986895
-          payload=Payload:
-           0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
-        
-        
-        ...can be accessed like dictionary:
-        dead
-        
-        
-        ...can be transformed into dictionary:
-        {'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
-        ```
-        
-        Next message:
-        ```python
-        '''
-        simple_message SimpleMessage ::= data : {
-            sequenceNumber    256,
-            swRelease  rel3,
-            payload {
-                'DEADBEEF'H
-            }
-        }
-        '''
-        data_payload = Payload()
-        data_payload.extend([Message(hexValue='DEADBEEF')])
-        
-        msg_data = Data()
-        msg_data['sequenceNumber'] = SequenceNumber(256)
-        msg_data['swRelease'] = Data.swRelease('rel3')
-        msg_data['payload'] = data_payload
-        
-        simple_message = SimpleMessage()
-        simple_message['data'] = msg_data
-        
-        per_bytes = encode(asn1Spec=simple_message)
-        print('encoded data bytes as hex string:')
-        print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
-        print('\n')
-        
-        decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
-        print('data message structure as string...:')
-        print(decoded)
-        print('...can be accessed like dictionary:')
-        print(decoded['data']['swRelease'])
-        print('\n')
-        
-        print('...can be transformed into dictionary:')
-        print(decoded.to_dict())
-        ```
-        
-        above will output:
-        ```
-        encoded data bytes as hex string:
-        60010043deadbeef
-        
-        
-        data message structure as string...:
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=256
-          swRelease=rel3
-          payload=Payload:
-           0xdeadbeef
-        
-        
-        ...can be accessed like dictionary:
-        rel3
-        
-        
-        ...can be transformed into dictionary:
-        {'data': OrderedDict([('sequenceNumber', 256), ('swRelease', 'rel3'), ('payload', ['deadbeef'])])}
-        ```
-        
-        ## Decoding from string
-        When encoded bytes are given as __string__ use _bytearray.fromhex()_:
-        
-        ```
-        
-        pure_string = str('70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb')
-        real_bytes = bytearray.fromhex(pure_string)
-        
-        decoded = decode(asn1Spec=SimpleMessage(), per_stream=real_bytes)
-        print(decoded)
-        ```
-        
-        above will output:
-        ```
-        SimpleMessage:
-         data=Data:
-          sequenceNumber=55555
-          swRelease=rel2
-          macroId=986895
-          payload=Payload:
-           0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
-        ```
-        
-        ## Dictionary creation
-          Data above can be accessed like dictionary but it is not a dictionary.
-          Method '__to_dict__' was added to make dictionary creation simple:
-        
-        ```
-        msg_dict = decoded.to_dict()
-        print(type(msg_dict))
-        print(msg_dict)
-        ```
-        
-        output:
-        ```
-        <class 'dict'>
-        {'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
-        ```
-        
-        To better show created structure, json.dumps() can be used:
-        ```
-        print(json.dumps(msg_dict, indent=2))
-        ```
-        
-        output:
-        ```
-        {
-          "data": {
-            "sequenceNumber": 55555,
-            "swRelease": "rel2",
-            "macroId": 986895,
-            "payload": [
-              "dead",
-              "beef",
-              "feed",
-              "aa",
-              "bbbbbbbb"
-            ]
-          }
-        }
-        ```
-        
-        ## Additional info
-        
-        For more examples please see library tests:
-        - parsing tests, located in test/parsing/ folder.
-        - coding/encoding tests, located in test/per folder.
-        
-        All above examples and tests where checked using:
-        https://asn1.io/asn1playground/
-        
-        This library inherits extensively from pyasn1 library so BER and other encoding should also work here.
-        
-        Parsing may take time - when trying to parse about 2000 lines of ASN.1 it took 15-20 minutes.
-        Tests for parsing also take time.
-        
-        ## History
-        
-        See CHANGES file.
-        
-        ## Known bugs
-        - Defining BitStringType type with default hexValue set to empty string (''), like:
-        ```
-        ...
-        d15     BIT STRING DEFAULT ''H,
-        ...
-        ```
-        will parse to Python code but running it will cause exception:
-        ```
-        pyasn1.error.PyAsn1Error: BitStringType.fromHexString() error: invalid literal for int() with base 16: ''
-        ```
-        
-        - This will parse, but sorting algorith may not sort it corretly:
-        ```
-            
-            MySeq2 ::= MySeq1   -- ok since one level of nesting is ok
-        
-            MySeq3 ::= MySeq1   -- ok since one level of nesting is ok
-            
-            MySeq1 ::= SEQUENCE {
-                d00     INTEGER
-            }
-        
-            MySeq4 ::= MySeq2   -- NOT OK! 2nd level of nesting 
-        ```
-        This will parse into:
-        ```python
-        MySeq4 = MySeq2
-        
-        
-        class MySeq1(SequenceType):
-            rootComponent = AdditiveNamedTypes(
-                NamedType('d00', IntegerType()),
-            )
-            componentType = rootComponent
-        
-        
-        MySeq3 = MySeq1
-        
-        
-        MySeq2 = MySeq1
-        ```
-        so Python will not find MySeq2 - this will lead to NameError.
-        
 Keywords: asn asn1 asn.1 PER decoder encoder
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# asn1PERser
+This library can parse ASN.1 text schemas into Python code. ASN.1 PER (Aligned) decoder/encoder is included to use with parsed schemas.
+
+Supported ASN.1 types and their constraints are:
+
+| ASN.1 Type   | Single value | Value range | Value size | can be extended (...) | used Python contraint class |
+|:------------:|:------------:|:-----------:|:----------:|:---------------------:|:---------------------------:|
+| INTEGER      |      X       |     X       |            |       X               |       ValueRange            |
+| BOOLEAN      |              |             |            |                       |                             |
+| ENUMERATED   |              |             |            |       X               |       ExtensionMarker       |
+| BIT STRING   |      X       |             |     X      |       X               |       ValueSize             |
+| OCTET STRING |      X       |             |     X      |       X               |       ValueSize             |
+| CHOICE       |              |             |            |       X               |       ExtensionMarker       |
+| SEQUENCE     |              |             |            |       X               |       ExtensionMarker       |
+| SEQUENCE OF  |      X       |             |     X      |       X               |       SequenceOfValueSize   |
+
+Table of contents:
+1. [Examples](#examples)
+2. [Decoding from string](#decoding-from-string)
+3. [Dictionary creation](#dictionary-creation)
+4. [Additional info](#additional-info)
+5. [History](#history)
+6. [Known bugs](#known-bugs)
+
+## Examples
+Following ASN.1 schema:
+
+```python
+asn_schema = '''\
+SimpleProtocol DEFINITIONS AUTOMATIC TAGS ::=
+BEGIN
+SimpleMessage ::= CHOICE {
+    start    Start,
+    stop     Stop,
+    alive    Alive,
+    data     Data,
+    ...
+}
+
+Start ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    timestamp         UTC-Timestamp,
+    srcPort           Port,
+    dstPort           Port
+}
+
+Stop ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    timestamp         UTC-Timestamp,
+    srcPort           Port,
+    dstPort           Port
+}
+
+Alive ::= SEQUENCE {
+    timestamp         UTC-Timestamp,
+    ...
+}
+
+Data ::= SEQUENCE {
+    sequenceNumber    SequenceNumber,
+    swRelease         ENUMERATED {rel1, rel2, rel3, ...},
+    macroId           BIT STRING (SIZE(20)) OPTIONAL,
+    payload           Payload
+}
+
+Port ::= INTEGER (10000..65535)
+
+SequenceNumber ::= INTEGER (0..65535)
+
+UTC-Timestamp ::= SEQUENCE {
+    seconds     INTEGER (0..4294967295),
+    useconds    INTEGER (0..4294967295)
+}
+
+Payload ::= SEQUENCE (SIZE(1..5)) OF Message
+
+Message ::= OCTET STRING (SIZE(1..4))
+
+END
+'''
+```
+
+can be parsed into Python code like this:
+```python
+from asn1PERser import parse_asn1_schema
+
+
+parse_asn1_schema(asn1_schema=asn_schema, output_folder=r'C:/my_code/')
+```
+
+Above code will create file 'SimpleProtocol.py' in folder (which must exist) 'C:/my_code/':
+```python
+from pyasn1.type.namedtype import NamedType, NamedTypes, OptionalNamedType, DefaultedNamedType
+from pyasn1.type.namedval import NamedValues
+from asn1PERser.classes.data.builtin import *
+from asn1PERser.classes.types.type import AdditiveNamedTypes
+from asn1PERser.classes.types.constraint import MIN, MAX, NoConstraint, ExtensionMarker, SequenceOfValueSize, \
+    ValueRange, SingleValue, ValueSize, ConstraintOr, ConstraintAnd
+
+
+class Port(IntegerType):
+    subtypeSpec = ValueRange(10000, 65535)
+
+
+class SequenceNumber(IntegerType):
+    subtypeSpec = ValueRange(0, 65535)
+
+
+class Message(OctetStringType):
+    subtypeSpec = ValueSize(1, 4)
+
+
+class UTC_Timestamp(SequenceType):
+    class seconds(IntegerType):
+        subtypeSpec = ValueRange(0, 4294967295)
+
+    class useconds(IntegerType):
+        subtypeSpec = ValueRange(0, 4294967295)
+
+    rootComponent = AdditiveNamedTypes(
+        NamedType('seconds', seconds()),
+        NamedType('useconds', useconds()),
+    )
+    componentType = rootComponent
+
+
+class Start(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('timestamp', UTC_Timestamp()),
+        NamedType('srcPort', Port()),
+        NamedType('dstPort', Port()),
+    )
+    componentType = rootComponent
+
+
+class Stop(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('timestamp', UTC_Timestamp()),
+        NamedType('srcPort', Port()),
+        NamedType('dstPort', Port()),
+    )
+    componentType = rootComponent
+
+
+class Alive(SequenceType):
+    subtypeSpec = ExtensionMarker(True)
+    rootComponent = AdditiveNamedTypes(
+        NamedType('timestamp', UTC_Timestamp()),
+    )
+    componentType = rootComponent
+
+
+class Payload(SequenceOfType):
+    subtypeSpec = SequenceOfValueSize(1, 5)
+    componentType = Message()
+
+
+class Data(SequenceType):
+    class swRelease(EnumeratedType):
+        subtypeSpec = ExtensionMarker(True)
+        enumerationRoot = NamedValues(
+            ('rel1', 0),
+            ('rel2', 1),
+            ('rel3', 2),
+        )
+        namedValues = enumerationRoot
+
+    class macroId(BitStringType):
+        subtypeSpec = ValueSize(20, 20)
+
+    rootComponent = AdditiveNamedTypes(
+        NamedType('sequenceNumber', SequenceNumber()),
+        NamedType('swRelease', swRelease()),
+        OptionalNamedType('macroId', macroId()),
+        NamedType('payload', Payload()),
+    )
+    componentType = rootComponent
+
+
+class SimpleMessage(ChoiceType):
+    subtypeSpec = ExtensionMarker(True)
+    rootComponent = AdditiveNamedTypes(
+        NamedType('start', Start()),
+        NamedType('stop', Stop()),
+        NamedType('alive', Alive()),
+        NamedType('data', Data()),
+    )
+    componentType = rootComponent
+
+
+
+```
+
+When schema is parsed it can be used - message can be created, encoded and decoded, using PER encoder/decoder, into bytes
+or Python structure:
+```python
+from asn1PERser import encode, decode
+from SimpleProtocol import *
+
+
+'''
+simple_message SimpleMessage ::= alive : {
+    timestamp {
+        seconds 1557528149,
+        useconds 12345
+    }
+}
+'''
+utc_timestamp = UTC_Timestamp()
+utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
+utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
+
+msg_alive = Alive()
+msg_alive['timestamp'] = utc_timestamp
+
+simple_message = SimpleMessage()
+simple_message['alive'] = msg_alive
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded alive bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('decoded alive message structure as string...:')
+print(decoded)
+
+print('...can be accessed like dictionary:')
+print(decoded['alive']['timestamp']['seconds'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded alive bytes as hex string:
+4c5cd5fe55403039
+
+
+decoded alive message structure as string...:
+SimpleMessage:
+ alive=Alive:
+  timestamp=UTC_Timestamp:
+   seconds=1557528149
+   useconds=12345
+
+
+
+...can be accessed like dictionary:
+1557528149
+
+
+...can be transformed into dictionary:
+{'alive': OrderedDict([('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)]))])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= start : {
+    sequenceNumber    10,
+    timestamp {
+        seconds 1557528149,
+        useconds 12345
+    },
+    srcPort    65533,
+    dstPort    10000
+}
+'''
+
+utc_timestamp = UTC_Timestamp()
+utc_timestamp['seconds'] = UTC_Timestamp.seconds(1557528149)
+utc_timestamp['useconds'] = UTC_Timestamp.useconds(12345)
+
+msg_start = Start()
+msg_start['sequenceNumber'] = SequenceNumber(10)
+msg_start['timestamp'] = utc_timestamp
+msg_start['srcPort'] = Port(65533)
+msg_start['dstPort'] = Port(10000)
+
+simple_message = SimpleMessage()
+simple_message['start'] = msg_start
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded start bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('start message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(decoded['start']['srcPort'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded start bytes as hex string:
+00000ac05cd5fe55403039d8ed0000
+
+
+start message structure as string...:
+SimpleMessage:
+ start=Start:
+  sequenceNumber=10
+  timestamp=UTC_Timestamp:
+   seconds=1557528149
+   useconds=12345
+
+  srcPort=65533
+  dstPort=10000
+
+
+...can be accessed like dictionary:
+65533
+
+
+...can be transformed into dictionary:
+{'start': OrderedDict([('sequenceNumber', 10), ('timestamp', OrderedDict([('seconds', 1557528149), ('useconds', 12345)])), ('srcPort', 65533), ('dstPort', 10000)])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= data : {
+    sequenceNumber    55555,
+    swRelease  rel2,
+    macroId    '11110000111100001111'B,
+    payload {
+        'DEAD'H,
+        'BEEF'H,
+        'FEED'H,
+        'AA'H,
+        'BBBBBBBB'H
+    }
+}
+'''
+
+data_payload = Payload()
+data_payload.extend([Message(hexValue='DEAD')])
+data_payload.extend([Message(hexValue='BEEF')])
+data_payload.extend([Message(hexValue='FEED')])
+data_payload.extend([Message(hexValue='AA')])
+data_payload.extend([Message(hexValue='BBBBBBBB')])
+
+msg_data = Data()
+msg_data['sequenceNumber'] = SequenceNumber(55555)
+msg_data['swRelease'] = Data.swRelease('rel2')
+msg_data['macroId'] = Data.macroId(binValue='11110000111100001111')
+msg_data['payload'] = data_payload
+
+simple_message = SimpleMessage()
+simple_message['data'] = msg_data
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded data bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('data message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(bytes(decoded['data']['payload'][0]).hex())
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded data bytes as hex string:
+70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb
+
+
+data message structure as string...:
+SimpleMessage:
+ data=Data:
+  sequenceNumber=55555
+  swRelease=rel2
+  macroId=986895
+  payload=Payload:
+   0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
+
+
+...can be accessed like dictionary:
+dead
+
+
+...can be transformed into dictionary:
+{'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
+```
+
+Next message:
+```python
+'''
+simple_message SimpleMessage ::= data : {
+    sequenceNumber    256,
+    swRelease  rel3,
+    payload {
+        'DEADBEEF'H
+    }
+}
+'''
+data_payload = Payload()
+data_payload.extend([Message(hexValue='DEADBEEF')])
+
+msg_data = Data()
+msg_data['sequenceNumber'] = SequenceNumber(256)
+msg_data['swRelease'] = Data.swRelease('rel3')
+msg_data['payload'] = data_payload
+
+simple_message = SimpleMessage()
+simple_message['data'] = msg_data
+
+per_bytes = encode(asn1Spec=simple_message)
+print('encoded data bytes as hex string:')
+print(per_bytes.hex())  # py2: print(binascii.hexlify(per_bytes))
+print('\n')
+
+decoded = decode(per_stream=per_bytes, asn1Spec=SimpleMessage())
+print('data message structure as string...:')
+print(decoded)
+print('...can be accessed like dictionary:')
+print(decoded['data']['swRelease'])
+print('\n')
+
+print('...can be transformed into dictionary:')
+print(decoded.to_dict())
+```
+
+above will output:
+```
+encoded data bytes as hex string:
+60010043deadbeef
+
+
+data message structure as string...:
+SimpleMessage:
+ data=Data:
+  sequenceNumber=256
+  swRelease=rel3
+  payload=Payload:
+   0xdeadbeef
+
+
+...can be accessed like dictionary:
+rel3
+
+
+...can be transformed into dictionary:
+{'data': OrderedDict([('sequenceNumber', 256), ('swRelease', 'rel3'), ('payload', ['deadbeef'])])}
+```
+
+## Decoding from string
+When encoded bytes are given as __string__ use _bytearray.fromhex()_:
+
+```
+
+pure_string = str('70d90320f0f0f880dead40beef40feed00aac0bbbbbbbb')
+real_bytes = bytearray.fromhex(pure_string)
+
+decoded = decode(asn1Spec=SimpleMessage(), per_stream=real_bytes)
+print(decoded)
+```
+
+above will output:
+```
+SimpleMessage:
+ data=Data:
+  sequenceNumber=55555
+  swRelease=rel2
+  macroId=986895
+  payload=Payload:
+   0xdead   0xbeef   0xfeed   0xaa   0xbbbbbbbb
+```
+
+## Dictionary creation
+  Data above can be accessed like dictionary but it is not a dictionary.
+  Method '__to_dict__' was added to make dictionary creation simple:
+
+```
+msg_dict = decoded.to_dict()
+print(type(msg_dict))
+print(msg_dict)
+```
+
+output:
+```
+<class 'dict'>
+{'data': OrderedDict([('sequenceNumber', 55555), ('swRelease', 'rel2'), ('macroId', 986895), ('payload', ['dead', 'beef', 'feed', 'aa', 'bbbbbbbb'])])}
+```
+
+To better show created structure, json.dumps() can be used:
+```
+print(json.dumps(msg_dict, indent=2))
+```
+
+output:
+```
+{
+  "data": {
+    "sequenceNumber": 55555,
+    "swRelease": "rel2",
+    "macroId": 986895,
+    "payload": [
+      "dead",
+      "beef",
+      "feed",
+      "aa",
+      "bbbbbbbb"
+    ]
+  }
+}
+```
+
+## Additional info
+
+For more examples please see library tests:
+- parsing tests, located in test/parsing/ folder.
+- coding/encoding tests, located in test/per folder.
+
+All above examples and tests where checked using:
+https://asn1.io/asn1playground/
+
+This library inherits extensively from pyasn1 library so BER and other encoding should also work here.
+
+Parsing may take time - when trying to parse about 2000 lines of ASN.1 it took 15-20 minutes.
+Tests for parsing also take time.
+
+asn1PERser uses logging library (for now only in decoder.py module).
+By default logging.NullHandler() is set as library top handler so no logs are visible.
+If you want to enable logging call asn1perser_logging_setup with (at least) handler
+parameter set to something else than logging.NullHandler:
+
+```
+import logging
+from asn1PERser import asn1perser_logging_setup
+
+asn1perser_logging_setup(logging.StreamHandler())
+```
+
+Above will print logging.INFO level logs to console.
+
+## History
+
+See CHANGES file.
+
+## Known bugs
+- Defining BitStringType type with default hexValue set to empty string (''), like:
+```
+...
+d15     BIT STRING DEFAULT ''H,
+...
+```
+will parse to Python code but running it will cause exception:
+```
+pyasn1.error.PyAsn1Error: BitStringType.fromHexString() error: invalid literal for int() with base 16: ''
+```
+
+- This will parse, but sorting algorith may not sort it corretly:
+```
+    
+    MySeq2 ::= MySeq1   -- ok since one level of nesting is ok
+
+    MySeq3 ::= MySeq1   -- ok since one level of nesting is ok
+    
+    MySeq1 ::= SEQUENCE {
+        d00     INTEGER
+    }
+
+    MySeq4 ::= MySeq2   -- NOT OK! 2nd level of nesting 
+```
+This will parse into:
+```python
+MySeq4 = MySeq2
+
+
+class MySeq1(SequenceType):
+    rootComponent = AdditiveNamedTypes(
+        NamedType('d00', IntegerType()),
+    )
+    componentType = rootComponent
+
+
+MySeq3 = MySeq1
+
+
+MySeq2 = MySeq1
+```
+so Python will not find MySeq2 - this will lead to NameError.
```

### Comparing `asn1PERser-0.4.2/README.md` & `asn1PERser-0.4.3/asn1PERser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: asn1PERser
+Version: 0.4.3
+Summary: Parse ASN.1 schemas into Python code and encode/decode them using PER encoder
+Home-page: https://github.com/erupikus/asn1PERser
+Author: Maciej Pikuła
+Author-email: erupikus@gmail.com
+Keywords: asn asn1 asn.1 PER decoder encoder
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # asn1PERser
 This library can parse ASN.1 text schemas into Python code. ASN.1 PER (Aligned) decoder/encoder is included to use with parsed schemas.
 
 Supported ASN.1 types and their constraints are:
 
 | ASN.1 Type   | Single value | Value range | Value size | can be extended (...) | used Python contraint class |
 |:------------:|:------------:|:-----------:|:----------:|:---------------------:|:---------------------------:|
@@ -533,14 +550,28 @@
 https://asn1.io/asn1playground/
 
 This library inherits extensively from pyasn1 library so BER and other encoding should also work here.
 
 Parsing may take time - when trying to parse about 2000 lines of ASN.1 it took 15-20 minutes.
 Tests for parsing also take time.
 
+asn1PERser uses logging library (for now only in decoder.py module).
+By default logging.NullHandler() is set as library top handler so no logs are visible.
+If you want to enable logging call asn1perser_logging_setup with (at least) handler
+parameter set to something else than logging.NullHandler:
+
+```
+import logging
+from asn1PERser import asn1perser_logging_setup
+
+asn1perser_logging_setup(logging.StreamHandler())
+```
+
+Above will print logging.INFO level logs to console.
+
 ## History
 
 See CHANGES file.
 
 ## Known bugs
 - Defining BitStringType type with default hexValue set to empty string (''), like:
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `asn1PERser-0.4.2/setup.py` & `asn1PERser-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asn1PERser",
-    version="0.4.2",
+    version="0.4.3",
     author="Maciej Pikuła",
     author_email="erupikus@gmail.com",
     description="Parse ASN.1 schemas into Python code and encode/decode them using PER encoder",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erupikus/asn1PERser",
     keywords = "asn asn1 asn.1 PER decoder encoder",
```


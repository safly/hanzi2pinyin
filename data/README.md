Refer to the Unicode standard chapter 12 for more information about the Unified
CJK Ideographs. Table 12-2 has the codepoint range for different blocks.

Notes for the codepoint to pinyin map files

- Unihan/unihan-codepoint2py.txt
  - The data is from the Unihan database
    ftp://ftp.unicode.org/Public/UNIDATA/Unihan.zip, unicode version 6.0.0
  - Created the pinyin mapping file from Unihan\_Readings.txt
  - More details in Unihan/process-unihan-readings.rb

At first I tried to use data from other sources, but these data has some
problems. Just document the experience here, data is not included.

- fcitx
  - Data file ``gbkpy.org`` in fcitx
  - Covers GBK character set, only one character is not in the 1st block
  - Problem: some characters have weird pinyin (maybe used in dialect)
- chinese\_pinyin from https://github.com/flyerhzm/chinese\_pinyin
  - Data file ``Mandarin.dat``
  - Contains the characters in the 1st block, extension A and B
  - Problem: the 1st block characters are not completely covered. Some
    characters covered in fcitx's data file is not present in this one.

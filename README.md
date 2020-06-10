# json5_parser
һ��֧��**json5**��json��������<br>��������DOM���Ϊ�������֣��Ա����ⲿ����DOMʵ�֡�<br>

����ͨ������ **JSON_ENABLE_JSON5** �����Ƿ�֧��**json5**��<br>

#### һ������

Ŀǰ��֪���⣺���ַ�����׼֧�ֽ�����<br>

#### ����Ч��

��I7 8700K 3.7GHz(OC 4.3GHz)��ʹ��VS 2019 / clang 9.0.0����(ȡ�ɼ��õı����������������dataĿ¼�¸���������json������������£�<br>

###### 1���ر�json5ѡ�����simdѡ��
```
dummy
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 2.01487 s, speeds is 852.372 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.42715 s, speeds is 1127.96 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.845587 s, speeds is 1558.39 MB/s

DOM
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 2.40061 s, speeds is 715.41 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.458313 s, speeds is 1051.26 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.914645 s, speeds is 1440.73 MB/s

benchmark_rapidjson parse file: ./data/canada.json
parse 2251060 bytes cost 2.91519 s, speeds is 589.128 MB/s
benchmark_rapidjson parse file: ./data/twitter.json
parse 631514 bytes cost 1.20984 s, speeds is 398.239 MB/s
benchmark_rapidjson parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 1.48519 s, speeds is 887.261 MB/s
```
עһ��dummy�����Խ�������Ч�ʣ��������κν��������

ע����DOM�ɸ�����JSON_DOMWalkerʵ�֣�û����ȷת���ַ�����������Ҫ���ٶ�λjson�á�

<br>

| ��Ŀ                | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :------------------ | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser(dummy) | clang  | canada.json       |      2251060      |   800    | 2.01487  | **852.372** |
| json5_parser(dummy) | clang  | twitter.json      |      631514       |   800    | 0.42715  | **1127.96** |
| json5_parser(dummy) | clang  | citm_catalog.json |      1727204      |   800    | 0.845587 | **1558.39** |
| json5_parser(DOM)   | clang  | canada.json       |      2251060      |   800    | 2.40061  | **715.41**  |
| json5_parser(DOM)   | clang  | twitter.json      |      631514       |   800    | 0.458313 | **1051.26** |
| json5_parser(DOM)   | clang  | citm_catalog.json |      1727204      |   800    | 0.914645 | **1440.73** |
| rapidjson           | clang  | canada.json       |      2251060      |   800    | 2.91519  | **589.128** |
| rapidjson           | clang  | twitter.json      |      631514       |   800    | 1.20984  | **398.239** |
| rapidjson           | clang  | citm_catalog.json |      1727204      |   800    | 1.48519  | **887.261** |

<br>

###### 2������json5ѡ�����simdѡ��
```
dummy
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 2.37301 s, speeds is 723.732 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.453873 s, speeds is 1061.55 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 1.00962 s, speeds is 1305.19 MB/s

DOM
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 2.55664 s, speeds is 671.749 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.473795 s, speeds is 1016.91 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 1.08489 s, speeds is 1214.64 MB/s
```
<br>

| ��Ŀ                | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :------------------ | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser(dummy) | clang  | canada.json       |      2251060      |   800    | 2.37301  | **723.732** |
| json5_parser(dummy) | clang  | twitter.json      |      631514       |   800    | 0.453873 | **1061.55** |
| json5_parser(dummy) | clang  | citm_catalog.json |      1727204      |   800    | 1.00962  | **1305.19** |
| json5_parser(DOM)   | clang  | canada.json       |      2251060      |   800    | 2.55664  | **671.749** |
| json5_parser(DOM)   | clang  | twitter.json      |      631514       |   800    | 0.473795 | **1016.91** |
| json5_parser(DOM)   | clang  | citm_catalog.json |      1727204      |   800    | 1.08489  | **1214.64** |

<br>

����ϰ�ߣ���һ����棺

����㷢�����κ�bug���кõĽ��顢��ʹ�����в���֮���������ύ��issue��Ҳ����ֱ����ϵ����:

```
email: tearshark@163.net
QQ����Ⱥ: 296561497
```


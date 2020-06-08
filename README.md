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
parse 2251060 bytes cost 0.471473 s, speeds is 910.669 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.103502 s, speeds is 1163.76 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.217996 s, speeds is 1511.21 MB/s

DOM
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 0.556339 s, speeds is 771.752 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.10866 s, speeds is 1108.52 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.220677 s, speeds is 1492.85 MB/s

benchmark_rapidjson parse file: ./data/canada.json
parse 2251060 bytes cost 0.74908 s, speeds is 573.177 MB/s
benchmark_rapidjson parse file: ./data/twitter.json
parse 631514 bytes cost 0.304658 s, speeds is 395.367 MB/s
benchmark_rapidjson parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.37469 s, speeds is 879.227 MB/s
```
<br>

| ��Ŀ                | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :------------------ | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser(dummy) | clang  | canada.json       |      2251060      |   200    | 0.471473 | **910.669** |
| json5_parser(dummy) | clang  | twitter.json      |      631514       |   200    | 0.103502 | **1163.76** |
| json5_parser(dummy) | clang  | citm_catalog.json |      1727204      |   200    | 0.217996 | **1511.21** |
| json5_parser(DOM)   | clang  | canada.json       |      2251060      |   200    | 0.556339 | **771.752** |
| json5_parser(DOM)   | clang  | twitter.json      |      631514       |   200    | 0.10866  | **1108.52** |
| json5_parser(DOM)   | clang  | citm_catalog.json |      1727204      |   200    | 0.220677 | **1492.85** |
| rapidjson           | clang  | canada.json       |      2251060      |   200    | 0.74908  | **573.177** |
| rapidjson           | clang  | twitter.json      |      631514       |   200    | 0.304658 | **395.367** |
| rapidjson           | clang  | citm_catalog.json |      1727204      |   200    | 0.37469  | **879.227** |

<br>

###### 2������json5ѡ�����simdѡ��
```
dummy
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 0.522491 s, speeds is 821.748 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.115304 s, speeds is 1044.65 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.246969 s, speeds is 1333.92 MB/s

DOM
benchmark_json5_parser parse file: ./data/canada.json
parse 2251060 bytes cost 0.587434 s, speeds is 730.9 MB/s
benchmark_json5_parser parse file: ./data/twitter.json
parse 631514 bytes cost 0.116074 s, speeds is 1037.72 MB/s
benchmark_json5_parser parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.255583 s, speeds is 1288.97 MB/s
```
<br>

| ��Ŀ                | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :------------------ | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser(dummy) | clang  | canada.json       |      2251060      |   200    | 0.522491 | **821.748** |
| json5_parser(dummy) | clang  | twitter.json      |      631514       |   200    | 0.115304 | **1044.65** |
| json5_parser(dummy) | clang  | citm_catalog.json |      1727204      |   200    | 0.246969 | **1333.92** |
| json5_parser(DOM)   | clang  | canada.json       |      2251060      |   200    | 0.587434 |  **730.9**  |
| json5_parser(DOM)   | clang  | twitter.json      |      631514       |   200    | 0.116074 | **1037.72** |
| json5_parser(DOM)   | clang  | citm_catalog.json |      1727204      |   200    | 0.255583 | **1288.97** |

<br>

����ϰ�ߣ���һ����棺

����㷢�����κ�bug���кõĽ��顢��ʹ�����в���֮���������ύ��issue��Ҳ����ֱ����ϵ����:

```
email: tearshark@163.net
QQ����Ⱥ: 296561497
```


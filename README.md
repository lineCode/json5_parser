# json5_parser
һ��֧��**json5**��json��������<br>��������DOM���Ϊ�������֣��Ա����ⲿ����DOMʵ�֡�<br>

����ͨ������ **JSON_ENABLE_JSON5** �����Ƿ�֧��**json5**��<br>

#### һ������

Ŀǰ��֪���⣺���ַ�����׼֧�ֽ�����<br>

#### ����Ч��

��I7 8700K 3.7GHz(OC 4.3GHz)��ʹ��VS 2019 / clang 9.0.0����(ȡ�ɼ��õı����������������dataĿ¼�¸���������json������������£�<br>

###### 1���ر�json5ѡ��
```
dummy
benchmark_json5_parser parse file: .\data\canada.json
parse 2251060 bytes cost 0.706516 s, speeds is 607.708 MB/s
benchmark_json5_parser parse file: .\data\twitter.json
parse 631514 bytes cost 0.12996 s, speeds is 926.84 MB/s
benchmark_json5_parser parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.222991 s, speeds is 1477.36 MB/s

DOM
benchmark_json5_parser parse file: .\data\canada.json
parse 2251060 bytes cost 0.997353 s, speeds is 430.495 MB/s
benchmark_json5_parser parse file: .\data\twitter.json
parse 631514 bytes cost 0.138747 s, speeds is 868.142 MB/s
benchmark_json5_parser parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.24073 s, speeds is 1368.5 MB/s

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
| json5_parser(dummy) |  msvc  | canada.json       |      2251060      |   200    | 0.706516 | **607.708** |
| json5_parser(dummy) |  msvc  | twitter.json      |      631514       |   200    | 0.125344 | **926.84**  |
| json5_parser(dummy) |  msvc  | citm_catalog.json |      1727204      |   200    | 0.218263 | **1477.36** |
| json5_parser(DOM)   |  msvc  | canada.json       |      2251060      |   200    | 0.997353 | **430.495** |
| json5_parser(DOM)   |  msvc  | twitter.json      |      631514       |   200    | 0.138747 | **868.142** |
| json5_parser(DOM)   |  msvc  | citm_catalog.json |      1727204      |   200    | 0.24073  | **1368.5**  |
| rapidjson           | clang  | canada.json       |      2251060      |   200    | 0.74908  | **573.177** |
| rapidjson           | clang  | twitter.json      |      631514       |   200    | 0.304658 | **395.367** |
| rapidjson           | clang  | citm_catalog.json |      1727204      |   200    | 0.37469  | **879.227** |

<br>

###### 2������json5ѡ��
```
dummy
benchmark_json5_parser parse file: .\data\canada.json
parse 2251060 bytes cost 0.756322 s, speeds is 567.689 MB/s
benchmark_json5_parser parse file: .\data\twitter.json
parse 631514 bytes cost 0.158458 s, speeds is 760.148 MB/s
benchmark_json5_parser parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.299909 s, speeds is 1098.46 MB/s

DOM
benchmark_json5_parser parse file: .\data\canada.json
parse 2251060 bytes cost 1.04293 s, speeds is 411.682 MB/s
benchmark_json5_parser parse file: .\data\twitter.json
parse 631514 bytes cost 0.165559 s, speeds is 727.547 MB/s
benchmark_json5_parser parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.307497 s, speeds is 1071.35 MB/s
```
<br>

| ��Ŀ                | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :------------------ | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser(dummy) |  msvc  | canada.json       |      2251060      |   200    | 0.756322 | **567.689** |
| json5_parser(dummy) |  msvc  | twitter.json      |      631514       |   200    | 0.158458 | **760.148** |
| json5_parser(dummy) |  msvc  | citm_catalog.json |      1727204      |   200    | 0.299909 | **1098.46** |
| json5_parser(DOM)   |  msvc  | canada.json       |      2251060      |   200    | 1.04293  | **411.682** |
| json5_parser(DOM)   |  msvc  | twitter.json      |      631514       |   200    | 0.165559 | **727.547** |
| json5_parser(DOM)   |  msvc  | citm_catalog.json |      1727204      |   200    | 0.307497 | **1071.35** |

<br>

����ϰ�ߣ���һ����棺

����㷢�����κ�bug���кõĽ��顢��ʹ�����в���֮���������ύ��issue��Ҳ����ֱ����ϵ����:

```
email: tearshark@163.net
QQ����Ⱥ: 296561497
```


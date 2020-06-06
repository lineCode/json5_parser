# json5_parser
һ��֧��**json5**��json��������<br>

����ͨ������ **JSON_ENABLE_JSON5** �����Ƿ�֧��**json5**��<br>

##### һ������

Ŀǰ��֪���⣺���ַ�����׼֧�ֽ�����<br>

##### ����Ч��

��I7 8700K 3.7GHz(OC 4.3GHz)��ʹ��VS 2019 / clang 9.0.0����(ȡ�ɼ��õı����������������dataĿ¼�¸���������json������������£�<br>

###### 1���ر�json5ѡ��
```
benchmark_parser_json parse file: .\data\canada.json
parse 2251060 bytes cost 0.966729 s, speeds is 444.132 MB/s
benchmark_parser_json parse file: .\data\twitter.json
parse 631514 bytes cost 0.125344 s, speeds is 960.97 MB/s
benchmark_parser_json parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.218263 s, speeds is 1509.36 MB/s

benchmark_rapidjson parse file: ./data/canada.json
parse 2251060 bytes cost 0.72091 s, speeds is 595.575 MB/s
benchmark_rapidjson parse file: ./data/twitter.json
parse 631514 bytes cost 0.305112 s, speeds is 394.779 MB/s
benchmark_rapidjson parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.363635 s, speeds is 905.959 MB/s
```

| ��Ŀ         | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :----------- | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser |  msvc  | canada.json       |      2251060      |   200    | 0.966729 | **444.132** |
| json5_parser |  msvc  | twitter.json      |      631514       |   200    | 0.125344 | **960.97**  |
| json5_parser |  msvc  | citm_catalog.json |      1727204      |   200    | 0.218263 | **1509.36** |
| rapidjson    | clang  | canada.json       |      2251060      |   200    | 0.72091  | **595.575** |
| rapidjson    | clang  | twitter.json      |      631514       |   200    | 0.305112 | **394.779** |
| rapidjson    | clang  | citm_catalog.json |      1727204      |   200    | 0.363635 | **905.959** |

<br>

###### 2������json5ѡ��
```
benchmark_parser_json parse file: .\data\canada.json
parse 2251060 bytes cost 1.05525 s, speeds is 406.875 MB/s
benchmark_parser_json parse file: .\data\twitter.json
parse 631514 bytes cost 0.139481 s, speeds is 863.57 MB/s
benchmark_parser_json parse file: .\data\citm_catalog.json
parse 1727204 bytes cost 0.278296 s, speeds is 1183.77 MB/s
```

| ��Ŀ         | ������ | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :----------- | :----: | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser |  msvc  | canada.json       |      2251060      |   200    | 1.05525  | **406.875** |
| json5_parser |  msvc  | twitter.json      |      631514       |   200    | 0.139481 | **863.57**  |
| json5_parser |  msvc  | citm_catalog.json |      1727204      |   200    | 0.278296 | **1183.77** |

<br>

����ϰ�ߣ���һ����棺

����㷢�����κ�bug���кõĽ��顢��ʹ�����в���֮���������ύ��issue��Ҳ����ֱ����ϵ����:

```
email: tearshark@163.net
QQ����Ⱥ: 296561497
```


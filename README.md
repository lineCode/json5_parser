# json5_parser
һ��֧��**json5**��json��������<br>

����ͨ������ **JSON_ENABLE_JSON5** �����Ƿ�֧��**json5**��<br>

##### һ������

Ŀǰ��֪���⣺���ַ�����׼֧�ֽ�����<br>

##### ����Ч��

��I7 8700K 3.7GHz(OC 4.3GHz)��ʹ��clang 9.0.0���룬����dataĿ¼�¸���������json������������£�<br>

###### 1���ر�json5ѡ��
```
benchmark_parser_json parse file: ./data/canada.json
parse 2251060 bytes cost 0.648113 s, speeds is 331.235 MB/s
benchmark_parser_json parse file: ./data/twitter.json
parse 631514 bytes cost 0.053727 s, speeds is 1120.96 MB/s
benchmark_parser_json parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.120617 s, speeds is 1365.64 MB/s

benchmark_rapidjson parse file: ./data/canada.json
parse 2251060 bytes cost 0.377634 s, speeds is 568.481 MB/s
benchmark_rapidjson parse file: ./data/twitter.json
parse 631514 bytes cost 0.154151 s, speeds is 390.693 MB/s
benchmark_rapidjson parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.195189 s, speeds is 843.896 MB/s
```

| ��Ŀ         | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��) | �ٶ�(MB/S)  |
| :----------- | :---------------- | :---------------: | :------: | :------: | :---------: |
| json5_parser | canada.json       |      2251060      |   100    | 0.648113 | **331.235** |
| json5_parser | twitter.json      |      631514       |   100    | 0.053727 | **1120.96** |
| json5_parser | citm_catalog.json |      1727204      |   100    | 0.120617 | **1365.64** |
| rapidjson    | canada.json       |      2251060      |   100    | 0.377634 | **568.481** |
| rapidjson    | twitter.json      |      631514       |   100    | 0.154151 | **390.693** |
| rapidjson    | citm_catalog.json |      1727204      |   100    | 0.195189 | **843.896** |

<br>

###### 2������json5ѡ��
```
benchmark_parser_json parse file: ./data/canada.json
parse 2251060 bytes cost 0.756168 s, speeds is 283.902 MB/s
benchmark_parser_json parse file: ./data/twitter.json
parse 631514 bytes cost 0.0538533 s, speeds is 1118.33 MB/s
benchmark_parser_json parse file: ./data/citm_catalog.json
parse 1727204 bytes cost 0.116481 s, speeds is 1414.13 MB/s
```

| ��Ŀ         | json�ļ�          | �ļ���С��Bytes�� | �ظ����� | ��ʱ(��)  | �ٶ�(MB/S)  |
| :----------- | :---------------- | :---------------: | :------: | :-------: | :---------: |
| json5_parser | canada.json       |      2251060      |   100    | 0.756168  | **283.902** |
| json5_parser | twitter.json      |      631514       |   100    | 0.0538533 | **1118.33** |
| json5_parser | citm_catalog.json |      1727204      |   100    | 0.116481  | **1414.13** |

<br>

����ϰ�ߣ���һ����棺

����㷢�����κ�bug���кõĽ��顢��ʹ�����в���֮���������ύ��issue��Ҳ����ֱ����ϵ����:

```
email: tearshark@163.net
QQ����Ⱥ: 296561497
```


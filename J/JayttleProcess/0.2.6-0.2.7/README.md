# Comparing `tmp/JayttleProcess-0.2.6-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 57921 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-24 02:33 JayttleProcess/CommonDecorator.py
--rw-rw-rw-  2.0 fat    10765 b- defN 24-Apr-24 06:24 JayttleProcess/ComputerControl.py
+Zip file size: 60451 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-29 13:43 JayttleProcess/CommonDecorator.py
+-rw-rw-rw-  2.0 fat    10785 b- defN 24-Apr-26 14:47 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
--rw-rw-rw-  2.0 fat     6780 b- defN 24-Apr-23 15:04 JayttleProcess/FTPCommonUse.py
+-rw-rw-rw-  2.0 fat     6834 b- defN 24-Apr-29 06:01 JayttleProcess/FTPCommonUse.py
 -rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-24 02:33 JayttleProcess/JsonCommonManage.py
+-rw-rw-rw-  2.0 fat     3461 b- defN 24-Apr-28 07:21 JayttleProcess/MachineLearning.py
 -rw-rw-rw-  2.0 fat    39584 b- defN 24-Apr-24 13:25 JayttleProcess/RinexCommonManage.py
--rw-rw-rw-  2.0 fat    33601 b- defN 24-Apr-24 14:07 JayttleProcess/SQLCommonUse.py
--rw-rw-rw-  2.0 fat     9319 b- defN 24-Apr-25 06:25 JayttleProcess/TBCProcessCsv.py
--rw-rw-rw-  2.0 fat   121491 b- defN 24-Apr-25 06:25 JayttleProcess/TimeSeriesDataMethod.py
+-rw-rw-rw-  2.0 fat    34687 b- defN 24-Apr-29 13:43 JayttleProcess/SQLCommonUse.py
+-rw-rw-rw-  2.0 fat    13711 b- defN 24-Apr-29 13:43 JayttleProcess/TBCProcessCsv.py
+-rw-rw-rw-  2.0 fat   120199 b- defN 24-Apr-29 13:42 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      578 b- defN 24-Apr-25 06:26 JayttleProcess-0.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 06:26 JayttleProcess-0.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-25 06:26 JayttleProcess-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1221 b- defN 24-Apr-25 06:26 JayttleProcess-0.2.6.dist-info/RECORD
-14 files, 232687 bytes uncompressed, 55873 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat      601 b- defN 24-Apr-29 13:44 JayttleProcess-0.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 13:44 JayttleProcess-0.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-29 13:43 JayttleProcess-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1312 b- defN 24-Apr-29 13:44 JayttleProcess-0.2.7.dist-info/RECORD
+15 files, 240522 bytes uncompressed, 58261 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: JayttleProcess/FTPCommonUse.py
 Comment: 
 
 Filename: JayttleProcess/JsonCommonManage.py
 Comment: 
 
+Filename: JayttleProcess/MachineLearning.py
+Comment: 
+
 Filename: JayttleProcess/RinexCommonManage.py
 Comment: 
 
 Filename: JayttleProcess/SQLCommonUse.py
 Comment: 
 
 Filename: JayttleProcess/TBCProcessCsv.py
@@ -24,20 +27,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.2.6.dist-info/METADATA
+Filename: JayttleProcess-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.2.6.dist-info/WHEEL
+Filename: JayttleProcess-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.2.6.dist-info/top_level.txt
+Filename: JayttleProcess-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.2.6.dist-info/RECORD
+Filename: JayttleProcess-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/ComputerControl.py

```diff
@@ -268,7 +268,8 @@
         time.sleep(1) #等待
         move_and_click(168, 290) #单击第一个文件
         time.sleep(0.5) #等待
         move_and_click_with_shift(147, 376) #拖动并点击最后一个文件
         time.sleep(0.5) #等待
         right_click_and_press_D() #删除文件
 
+# TBC_auto_Process()
```

## JayttleProcess/FTPCommonUse.py

```diff
@@ -1,12 +1,15 @@
 import os
 from ftplib import FTP
 import json
+import datetime
+from dataclasses import dataclass
 import JayttleProcess.CommonDecorator as ComD
 
+
 class FTPConfig:
     def __init__(self, json_file_path: str):
         # 确保 JSON 文件存在
         if not os.path.exists(json_file_path):
             raise FileNotFoundError(f"指定的 JSON 文件不存在: {json_file_path}")
         
         # 从 JSON 文件中读取配置信息
```

## JayttleProcess/SQLCommonUse.py

```diff
@@ -766,14 +766,48 @@
     # 将表格输出到文件
     with open('output_table.txt', 'w', encoding='utf-8') as file:
         file.write(table)
 
     print("表格已经成功输出到文件 output_table.txt 中。")
 
 
+def export_data_availability_to_excel(daily_data_availability: dict[datetime, dict[str, float]]) -> None:
+    """
+    将每日数据存有率字典输出到 Excel 文件
+    
+    参数：
+        daily_data_availability (Dict[datetime, Dict[str, float]]): 包含日期和每日数据存有率的字典
+        
+    返回：
+        None
+    """
+    # 将字典转换为 DataFrame
+    df = pd.DataFrame.from_dict(daily_data_availability, orient='index')
+    
+    # 将 NaN 替换为 0
+    df = df.fillna(0)
+
+    # 将 0 的数据存有率标识为 'N/A'
+    df = df.applymap(lambda val: 'N/A' if val == 0 else val)
+
+    # 重置索引，使日期成为列
+    df.reset_index(inplace=True)
+    df.rename(columns={'index': 'Date'}, inplace=True)
+
+    # 排序日期
+    df['Date'] = pd.to_datetime(df['Date'])
+    df = df.sort_values('Date')
+
+    # 生成 Excel 文件
+    excel_filename = 'output_table.xlsx'
+    df.to_excel(excel_filename, index=False)
+
+    print(f"表格已经成功输出到 Excel 文件 {excel_filename} 中。")
+
+
 @log_function_call
 def load_missing_intervals(file_path: str) -> list[tuple[datetime, datetime, int]]:
     """
     从文件加载数据到 missing_intervals 列表中
     
     参数：
         file_path (str): 文件路径
@@ -798,16 +832,15 @@
 
             # 添加到 missing_intervals
             missing_intervals.append((start_time, end_time, missing_seconds))
 
     return missing_intervals
 
 
-
-
+@log_function_call
 def main() -> None:
     file_path_met = "D:/python_proj2/SQL_Met.txt"
     file_path_accelerometer = "D:/python_proj2/SQL_accelerometer.txt"
     file_path_tiltmeter = "D:/python_proj2/SQL_tiltmeter.txt"
     file_path_arr = "D:/python_proj2/SQL_arr.txt"
     file_path_ggkx = "D:/python_proj2/SQL_arr.txt"
 
@@ -863,15 +896,16 @@
             'daily_arr': daily_availability_arr.get(date, 0),
             'daily_ggkx': daily_availability_ggkx.get(date, 0),
             'daily_met': daily_availability_met.get(date, 0),    
             'daily_tiltmeter': daily_availability_tiltmeter.get(date, 0),
             'daily_accelerometer': daily_availability_accelerometer.get(date, 0),
         }
 
-    export_data_availability_to_file(combined_dict)
+    # export_data_availability_to_file(combined_dict)
+    export_data_availability_to_excel(combined_dict)
 
 
 def parse_tabulated_data(filepath):
     with open(filepath, 'r', encoding='utf-8') as file:
         lines = [line.rstrip() for line in file if line.strip()]
 
     # Determine the indices for header and data sections
@@ -937,45 +971,50 @@
     except Exception as e:
         print("Error executing SQL statement:", e)
         return None
     finally:
         cursor.close()
         conn.close()
 
-# file_path = "query_high_frequency_periods.txt"
 
-# # 用于存储时间和数值的字典
-# time_value_dict = {}
 
-# # 读取文件并提取时间和数值信息
-# with open(file_path, 'r') as file:
-#     for line in file:
-#         # 去除每行末尾的换行符
-#         line = line.strip()
-#         # 确保当前行不为空
-#         if line:
-#             # 按逗号分割当前行
-#             parts = line.split(', ')
-#             # 确保当前行包含两个部分：时间和数值
-#             if len(parts) == 2:
-#                 # 提取时间和数值
-#                 time_info = parts[0].strip("('")
-#                 value = int(parts[1].strip("')"))
-#                 # 将时间作为键，数值作为值添加到字典中
-#                 time_value_dict[time_info] = value
-
-
-# # 创建一个列表来存储符合条件的 time_info
-# selected_time_infos = []
-
-# # 遍历 time_value_dict，找出 value 大于 40 的 time_info，并添加到 selected_time_infos 列表中
-# for time_info, value in time_value_dict.items():
-#     if value > 40:
-#         selected_time_infos.append(time_info)
-
-# # 将符合条件的 time_info 写入到 txt 文件中
-# output_file_path = "selected_time_infos.txt"
-# with open(output_file_path, "w") as file:
-#     for time_info in selected_time_infos:
-#         file.write(time_info + "\n")
+def execute_sql_and_save_to_txt(sql_statement: str, file_path: str):
+    # 建立数据库连接
+    conn = pymysql.connect(**SQL_CONFIG)
+    cursor = conn.cursor()
+    
+    try:
+        # 执行输入的 SQL 语句
+        cursor.execute(sql_statement)
+        
+        # 如果是查询语句，则将查询结果写入到 txt 文件中
+        if sql_statement.strip().upper().startswith("SELECT"):
+            results = cursor.fetchall()
+            with open(file_path, 'w') as f:
+                for row in results:
+                    f.write(','.join(map(str, row)) + '\n')
+            return "Query executed successfully. Results saved to " + file_path
+        else:
+            # 提交更改
+            conn.commit()
+            return "SQL statement executed successfully!"
 
-# print("已将符合条件的 time_info 写入到文件:", output_file_path)
+    except Exception as e:
+        # 发生错误时回滚
+        conn.rollback()
+        return "Error executing SQL statement: " + str(e)
+
+    finally:
+        # 关闭游标和数据库连接
+        cursor.close()
+        conn.close()
+
+
+def Proj1_high_frequency_data():
+    # 执行 SQL 查询并将结果保存到指定的 txt 文件中
+    sql_statement = """
+    SELECT * FROM ggkx
+    WHERE time >= '2023-11-24 13:25:13' AND time <= '2023-12-04 14:16:10';
+    """
+    file_path = "SQLquery_results.txt"
+    result = execute_sql_and_save_to_txt(sql_statement, file_path)
+
```

## JayttleProcess/TBCProcessCsv.py

```diff
@@ -1,18 +1,28 @@
 import os
 import csv
 import pandas as pd
+import json
 import chardet
+import pyproj
+from datetime import datetime
+from collections import defaultdict
+from dataclasses import dataclass
+from typing import TypedDict, List, Dict, Optional
 from JayttleProcess import CommonDecorator
 from JayttleProcess import TimeSeriesDataMethod as TSD
 from JayttleProcess.TimeSeriesDataMethod import TimeSeriesData
 
 
-#csv文件的编码格式 全局变量
-encoding = None
+# region  全局变量
+encoding = None # csv文件的编码格式 全局变量
+datapoints_csv = [] # 读取的csv点数据存储
+json_data = None  # 初始化为 None 或者其他默认值
+# endregion
+
 
 class DataPoint:
     def __init__(self, point_id: str, north_coordinate: float, east_coordinate: float, elevation: float,
                  latitude: float, longitude: float, ellipsoid_height: float, start_time: str, end_time: str,
                  duration: str, pdop: float, rms: float, horizontal_accuracy: float, vertical_accuracy: float,
                  north_coordinate_error: float, east_coordinate_error: float, elevation_error: float,
                  height_error: str):
@@ -121,15 +131,15 @@
     if selected_value is None:
         return None
     # 将 datapoint.start_time 转换为字符串
     start_time_str = str(datapoint.start_time)
     return TimeSeriesData(selected_value, start_time_str)
 
 
-def export_list_to_excel(datapoints: list[DataPoint]):
+def export_list_to_excel(datapoints: list[DataPoint]) -> None:
     # 将 DataPoint 对象列表转换为 Pandas DataFrame
     datapoints_df = pd.DataFrame([vars(dp) for dp in datapoints])
 
     # 将 start_time 转换为日期并设置为索引
     datapoints_df['start_time'] = pd.to_datetime(datapoints_df['start_time'])
     datapoints_df.set_index(datapoints_df['start_time'].dt.date, inplace=True)
 
@@ -158,26 +168,150 @@
     # 输出填充后的 DataFrame 到 Excel 文件
     output_excel_path = "filled_datapoints.xlsx"
     filled_df.to_excel(output_excel_path)
 
     print("已将填充后的数据导出到 Excel 文件:", output_excel_path)
 
 
+class Coordinates(TypedDict):
+    Lat: float
+    Lon: float
+    GeoHeight: float
+
+class Correction(TypedDict):
+    Distance: float
+    TiltAngle: float
+    TorsionAngle: float
+
+class Threshold(TypedDict):
+    Distance: float
+    Tilt: float
+    Torsion: float
+
+class Data(TypedDict):
+    GaussOption: Dict[str, float]
+    CablewayOption: Dict[str, float]
+    MaxDiffLength: float
+    MaxDiffDistance: float
+    Thresholds: List[Threshold]
+    Coors: Dict[str, List[Coordinates]]
+    Corrections: Dict[str, Correction]
+
+def read_json_file(file_path: str) -> Data:
+    with open(file_path, 'r') as file:
+        data = json.load(file)
+    return data
+
+
+
+def convert_coordinates(lat: float, lon: float) -> tuple[float, float]:
+    # 定义原始坐标系（WGS84）
+    from_proj = pyproj.Proj(proj='latlong', datum='WGS84')
+
+    # 定义目标投影坐标系（例如，Transverse Mercator投影）
+    to_proj_params = {
+        'proj': 'tmerc',
+        'lat_0': 0,
+        'lon_0': 117,
+        'k': 1,
+        'x_0': 500000,
+        'y_0': 0,
+        'ellps': 'WGS84',
+        'units': 'm'
+    }
+    to_proj = pyproj.Proj(to_proj_params)
+
+    # 执行坐标转换
+    easting, northing = pyproj.transform(from_proj, to_proj, lon, lat)
+
+    return easting, northing
+
+
+@dataclass
+class GgkxDto:
+    Time: datetime
+    StationId: int
+    ReceiverId: int
+    Lat: float
+    Lon: float
+    GeoHeight: float
+    FixMode: int
+    SateNum: int
+    Pdop: float
+    SigmaE: float
+    SigmaN: float
+    SigmaU: float
+    Prop_Age: float
+
+# 使用 defaultdict 创建一个字典，值的默认类型是列表
+data_dict: dict[str, list[GgkxDto]] = defaultdict(list)
+
+@CommonDecorator.log_function_call
+def read_data(file_path: str) -> None:
+    with open(file_path, 'r') as file:
+        for line in file:
+            row = line.strip().split(',')
+            time_format = '%Y-%m-%d %H:%M:%S.%f' if '.' in row[0] else '%Y-%m-%d %H:%M:%S'
+            time = datetime.strptime(row[0], time_format)
+            station_id = int(row[1])
+            receiver_id = int(row[2])
+            lat = float(row[3])
+            lon = float(row[4])
+            geo_height = float(row[5])
+            fix_mode = int(row[6])
+            sate_num = int(row[7])
+            pdop = float(row[8])
+            sigma_e = float(row[9])
+            sigma_n = float(row[10])
+            sigma_u = float(row[11])
+            prop_age = float(row[12])
+            ggkx = GgkxDto(time, station_id, receiver_id, lat, lon, geo_height, fix_mode, sate_num, pdop, sigma_e, sigma_n, sigma_u, prop_age)
+            # 将数据添加到字典中对应的列表中
+            key = f'{station_id}{receiver_id}'
+            data_dict[key].append(ggkx)
+
 
-csv_folder_path = r'D:\Ropeway\FTPcsv'
-datapoints = []
+@CommonDecorator.log_function_call
+def do_porj1() -> None:
+    # 读取数据
+    read_data(r"D:\Program Files (x86)\Software\OneDrive\PyPackages\8_data.txt")
+
+    # 将数据按照 station_id 和 receiver_id 写入到本地 txt 文件中
+    for key, ggkx_list in data_dict.items():
+        with open(f"R0{key}_data.txt", 'w') as f:
+            for ggkx in ggkx_list:
+                f.write(f"{ggkx.Time},{ggkx.StationId},{ggkx.ReceiverId},{ggkx.Lat},{ggkx.Lon},{ggkx.GeoHeight},{ggkx.FixMode},{ggkx.SateNum},{ggkx.Pdop},{ggkx.SigmaE},{ggkx.SigmaN},{ggkx.SigmaU},{ggkx.Prop_Age}\n")
 
-# Iterate through each CSV file in the folder
-for filename in os.listdir(csv_folder_path):
-    if filename.endswith('.csv'):
-        csv_file_path = os.path.join(csv_folder_path, filename)
-        datapoints.extend(read_csv_to_datapoints(csv_file_path))
-
-# 定义要提取的属性键
-value_key = "north_coordinate"
-# 使用列表推导式创建 TimeSeriesData 对象列表
-my_tsd: list[TimeSeriesData] = [create_timeseries_data(datapoint, value_key) for datapoint in datapoints]
-TSD.remove_average(my_tsd)
-TSD.plot_TimeSeriesData_in_threshold(my_tsd, 100, True)
 
+@CommonDecorator.log_function_call
+def before_process_proj() -> None:
+    json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\config.json'
+    json_data: Data = read_json_file(json_file_path)
 
+    
+    # 输入经度和纬度坐标
+    lat: float = 35.474245973695
+    lon: float = 118.042930824340
+
+    # 执行坐标转换
+    easting, northing = convert_coordinates(lat, lon)
+    print(f'easting:{easting}\tnorthing:{northing}')
+
+
+    global datapoints_csv
+    # 现在你可以使用这些数据进行进一步的处理
+    csv_folder_path = r'D:\Ropeway\FTPCsv3'
+    # Iterate through each CSV file in the folder
+    for filename in os.listdir(csv_folder_path):
+        if filename.endswith('.csv'):
+            csv_file_path = os.path.join(csv_folder_path, filename)
+            datapoints_csv.extend(read_csv_to_datapoints(csv_file_path))
+
+    export_list_to_excel(datapoints_csv)
+
+    # 定义要提取的属性键
+    value_key = "north_coordinate"
+    # 使用列表推导式创建 TimeSeriesData 对象列表
+    my_tsd: list[TimeSeriesData] = [create_timeseries_data(datapoint, value_key) for datapoint in datapoints_csv]
+    TSD.remove_average(my_tsd)
+    # TSD.plot_TimeSeriesData_threshold(my_tsd, True, threshold = 100)
```

## JayttleProcess/TimeSeriesDataMethod.py

```diff
@@ -87,20 +87,24 @@
         time_series_data.append(data)
     return time_series_data
 
 
 def remove_average(TimeSeriesData: list[TimeSeriesData]) -> None:
     """对时序数据进行去平均 再乘以1000"""
     mean_value = np.mean([point.value for point in TimeSeriesData])
-    # 减去平均值
-    for point in TimeSeriesData:
-        point.value -= mean_value
-        point.value = point.value * 1000
+    remove_specific_value(TimeSeriesData, mean_value)
 
 
+def remove_specific_value(TimeSeriesData: List[TimeSeriesData], specific_value: float) -> None:
+    """对时序数据进行减去特定值 再乘以1000"""
+    # 减去平均值并乘以1000
+    for point in TimeSeriesData:
+        point.value = (point.value - specific_value) * 1000
+    
+
 def plot_TimeSeriesData(TimeSeriesData: list[TimeSeriesData], isShow: bool = False, SaveFilePath: Optional[str] = None) -> None:
     """绘制TimeSeriesData对象的时间序列图"""
     values = [data.value for data in TimeSeriesData]
     datetimes = [data.datetime for data in TimeSeriesData]
 
     # 修改标签和标题的文本为中文
     plt.figure(figsize=(14.4, 9.6)) # 单位是英寸
@@ -123,64 +127,14 @@
     if SaveFilePath is not None:
         plt.savefig(SaveFilePath)
     elif isShow:
         plt.show()
     plt.close()
 
 
-def plot_TimeSeriesData_in_threshold(TimeSeriesData: list[TimeSeriesData], threshold: float, isShow: bool = False, SaveFilePath: Optional[str] = None) -> None:
-    """绘制TimeSeriesData对象的时间序列图"""
-    values = [data.value for data in TimeSeriesData]
-    datetimes = [data.datetime for data in TimeSeriesData]
-
-    # 修改标签和标题的文本为中文
-    plt.figure(figsize=(25.6, 14.4))  # 单位是英寸
-    plt.xlabel('日期')
-    plt.ylabel('数值')
-    plt.title('时间序列数据')
-
-    # 设置日期格式化器和日期刻度定位器
-    date_fmt = mdates.DateFormatter("%m-%d")  # 仅显示月-日
-    date_locator = mdates.AutoDateLocator()  # 自动选择刻度间隔
-    plt.gca().xaxis.set_major_formatter(date_fmt)
-    plt.gca().xaxis.set_major_locator(date_locator)
-    
-    # 设置最大显示的刻度数
-    plt.gcf().autofmt_xdate()  # 旋转日期标签以避免重叠
-    plt.tight_layout()  # 自动调整子图间的间距和标签位置
-
-    # 创建一个新列表，用于存储将要绘制的数据
-    filtered_values = []
-    filtered_datetimes = []
-
-    for i in range(len(TimeSeriesData) - 1):
-        # 计算相邻数据点之间的时间差
-        time_diff = (datetimes[i + 1] - datetimes[i]).total_seconds()
-
-        # 如果时间差大于阈值，则将当前数据点和下一个数据点都设置为 NaN
-        if time_diff > threshold:
-            filtered_values.extend([values[i], float('nan')])
-            filtered_datetimes.extend([datetimes[i], datetimes[i + 1]])
-        else:
-            filtered_values.append(values[i])
-            filtered_datetimes.append(datetimes[i])
-
-    # 将最后一个数据点添加到过滤后的列表中
-    filtered_values.append(values[-1])
-    filtered_datetimes.append(datetimes[-1])
-
-    plt.plot(filtered_datetimes, filtered_values)
-
-    if SaveFilePath is not None:
-        plt.savefig(SaveFilePath)
-    elif isShow:
-        plt.show()
-    plt.close()
-
-
 def plot_TimeSeriesData_Compare(TimeSeriesData1: list[TimeSeriesData], TimeSeriesData2: list[TimeSeriesData], SaveFilePath: Optional[str] = None) -> None:
     """绘制两个TimeSeriesData对象的时间序列图"""
     values1 = [data.value for data in TimeSeriesData1]
     datetimes1 = [data.datetime for data in TimeSeriesData1]
 
     values2 = [data.value for data in TimeSeriesData2]
 
@@ -266,14 +220,25 @@
         current_value = time_series_data[i].value
         previous_value = time_series_data[i-1].value
         change_rate = (current_value - previous_value) / previous_value
         change_rates.append(change_rate)
     return change_rates
 
 
+def calculate_correlation(data1: List[TimeSeriesData], data2: List[TimeSeriesData]) -> float:
+    # 转换为 Pandas DataFrame
+    df1 = pd.DataFrame([(ts.datetime, ts.value) for ts in data1], columns=['Datetime', 'Value']).set_index('Datetime')
+    df2 = pd.DataFrame([(ts.datetime, ts.value) for ts in data2], columns=['Datetime', 'Value']).set_index('Datetime')
+    
+    # 使用 Pandas 的 corr 方法计算相关性
+    correlation = df1.corrwith(df2, axis=0).iloc[0]
+    
+    return correlation
+
+
 def get_x_values(data: list[TimeSeriesData]) -> List[int]:
     """获取时间步作为x值"""
     # 获取时间步作为x值
     x = []
     for i in range(len(data)):
         x.append(i)
     return x
```

## Comparing `JayttleProcess-0.2.6.dist-info/METADATA` & `JayttleProcess-0.2.7.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.2.6
-Summary: modifty time:2024-04-25 14:25
+Version: 0.2.7
+Summary: modifty time:2024-04-29 21:25
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
@@ -17,11 +17,12 @@
 Requires-Dist: PyWavelets
 Requires-Dist: pymysql
 Requires-Dist: numpy
 Requires-Dist: seaborn
 Requires-Dist: pandas
 Requires-Dist: openpyxl
 Requires-Dist: chardet
+Requires-Dist: pyproj
 
 UNKNOWN
```

## Comparing `JayttleProcess-0.2.6.dist-info/RECORD` & `JayttleProcess-0.2.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 JayttleProcess/CommonDecorator.py,sha256=ES7hIDpAL3zhzpJYEXlgG4_LGvDsBoJqgIcruJiIr9A,2978
-JayttleProcess/ComputerControl.py,sha256=G-MGLHPKLXxTC1uv6KSqL2A3BjcSSUt7t5DbsoZaYgc,10765
+JayttleProcess/ComputerControl.py,sha256=xm-Z3JxJNdZP86SPXvGcZ3-dOyL12Zs9wqmFatOR2iU,10785
 JayttleProcess/EntertainmentCode.py,sha256=KR-nFHjwIjfl8E_IMuRl44p2Xwkw6UMZYuvkdL9NFck,613
-JayttleProcess/FTPCommonUse.py,sha256=gpniZo2IAqyOWsuqh3NIsZ0ON6vfAHJBcIR3tVLX7zs,6780
+JayttleProcess/FTPCommonUse.py,sha256=awsRf0Dm0faUCdI3dW8FNg2bZWGT1bRd3MNcPIfhttA,6834
 JayttleProcess/JsonCommonManage.py,sha256=KJtfAxPUGktFMocoFKFd8E_VtGW-vyhAMPPz--34mkA,5650
+JayttleProcess/MachineLearning.py,sha256=Xi3iI7woakrlusNqFhoVHznpuwntUt9YUeWIZTLP2MI,3461
 JayttleProcess/RinexCommonManage.py,sha256=bDOK6YLqXYSD4shuKzioDZxuNhgubfKYp8VLMVZFfZ4,39584
-JayttleProcess/SQLCommonUse.py,sha256=EYfkANgm8Gk5isOpwAcL1ZwIQW6k_tSUyNdeiZLLoYc,33601
-JayttleProcess/TBCProcessCsv.py,sha256=sSwa50ggrqmt4c55DvC0ZszY5eqpKgD_lU_pbd8p1VY,9319
-JayttleProcess/TimeSeriesDataMethod.py,sha256=BRp5IfXsLR7_t22Gafz8T2y6C82ykRShJy73Mrp-iwU,121491
+JayttleProcess/SQLCommonUse.py,sha256=PZe1IgQ60ZQYDbCU-f_z_kt4uBDBXlJQboa-niiixV4,34687
+JayttleProcess/TBCProcessCsv.py,sha256=nx5yUpGaQ-CJDBueMq0uglQxYeY_a2Z2S_9fRzqshLY,13711
+JayttleProcess/TimeSeriesDataMethod.py,sha256=8remneGfzgSvQ6ni4aHa045b86GhYPffwNKDPRIs8uI,120199
 JayttleProcess/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-JayttleProcess-0.2.6.dist-info/METADATA,sha256=e4rcEM2vLDgshq1i90KHbLWH2Tjs7DqM0d8wapJP2dk,578
-JayttleProcess-0.2.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-JayttleProcess-0.2.6.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
-JayttleProcess-0.2.6.dist-info/RECORD,,
+JayttleProcess-0.2.7.dist-info/METADATA,sha256=yjv-xsVgelGI3iHHNfpKxU-csMdcEEGoz69u7NV9_Uk,601
+JayttleProcess-0.2.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+JayttleProcess-0.2.7.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
+JayttleProcess-0.2.7.dist-info/RECORD,,
```


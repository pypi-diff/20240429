# Comparing `tmp/sswater-0.0.3.tar.gz` & `tmp/sswater-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sswater-0.0.3.tar", last modified: Wed Apr 17 08:04:06 2024, max compression
+gzip compressed data, was "sswater-0.0.4.tar", last modified: Mon Apr 29 06:00:21 2024, max compression
```

## Comparing `sswater-0.0.3.tar` & `sswater-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.998079 sswater-0.0.3/
--rw-rw-rw-   0        0        0      341 2024-04-17 08:04:05.997077 sswater-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-17 08:04:05.998079 sswater-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      509 2024-04-17 08:04:02.000000 sswater-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.985602 sswater-0.0.3/sswater/
--rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.3/sswater/GAILinear.py
--rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.3/sswater/NLinear.py
--rw-rw-rw-   0        0        0       21 2024-04-17 08:03:57.000000 sswater-0.0.3/sswater/__init__.py
--rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.3/sswater/config.py
--rw-rw-rw-   0        0        0      679 2024-03-18 05:21:00.000000 sswater-0.0.3/sswater/create_seq.py
--rw-rw-rw-   0        0        0     3437 2024-04-17 07:49:37.000000 sswater-0.0.3/sswater/preprocessing.py
--rw-rw-rw-   0        0        0     4352 2024-04-17 07:57:47.000000 sswater-0.0.3/sswater/services.py
--rw-rw-rw-   0        0        0     3858 2024-04-17 07:34:50.000000 sswater-0.0.3/sswater/train.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:04:05.995078 sswater-0.0.3/sswater.egg-info/
--rw-rw-rw-   0        0        0      341 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-15 08:18:40.000000 sswater-0.0.3/sswater.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       32 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 08:04:05.000000 sswater-0.0.3/sswater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 06:00:21.883513 sswater-0.0.4/
+-rw-rw-rw-   0        0        0      341 2024-04-29 06:00:21.881512 sswater-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:00:21.883513 sswater-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      509 2024-04-29 05:55:24.000000 sswater-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:00:21.869990 sswater-0.0.4/sswater/
+-rw-rw-rw-   0        0        0     3566 2024-03-18 02:10:44.000000 sswater-0.0.4/sswater/GAILinear.py
+-rw-rw-rw-   0        0        0     1437 2024-03-28 00:19:20.000000 sswater-0.0.4/sswater/NLinear.py
+-rw-rw-rw-   0        0        0       21 2024-04-29 05:55:30.000000 sswater-0.0.4/sswater/__init__.py
+-rw-rw-rw-   0        0        0      490 2024-02-06 07:46:54.000000 sswater-0.0.4/sswater/config.py
+-rw-rw-rw-   0        0        0      442 2024-04-22 08:34:52.000000 sswater-0.0.4/sswater/create_seq.py
+-rw-rw-rw-   0        0        0      622 2024-04-17 00:50:30.000000 sswater-0.0.4/sswater/models.py
+-rw-rw-rw-   0        0        0     3709 2024-04-29 05:54:34.000000 sswater-0.0.4/sswater/preprocessing.py
+-rw-rw-rw-   0        0        0      862 2024-04-23 07:31:56.000000 sswater-0.0.4/sswater/serializers.py
+-rw-rw-rw-   0        0        0     4653 2024-04-29 05:45:24.000000 sswater-0.0.4/sswater/services.py
+-rw-rw-rw-   0        0        0     3963 2024-04-22 09:12:50.000000 sswater-0.0.4/sswater/train.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:00:21.879514 sswater-0.0.4/sswater.egg-info/
+-rw-rw-rw-   0        0        0      341 2024-04-29 06:00:21.000000 sswater-0.0.4/sswater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-04-29 06:00:21.000000 sswater-0.0.4/sswater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:00:21.000000 sswater-0.0.4/sswater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 08:18:40.000000 sswater-0.0.4/sswater.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       32 2024-04-29 06:00:21.000000 sswater-0.0.4/sswater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 06:00:21.000000 sswater-0.0.4/sswater.egg-info/top_level.txt
```

### Comparing `sswater-0.0.3/sswater/GAILinear.py` & `sswater-0.0.4/sswater/GAILinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.3/sswater/NLinear.py` & `sswater-0.0.4/sswater/NLinear.py`

 * *Files identical despite different names*

### Comparing `sswater-0.0.3/sswater/preprocessing.py` & `sswater-0.0.4/sswater/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pymysql
+from sqlalchemy import create_engine
 import pandas as pd
 from datetime import datetime, timedelta
 from sklearn.preprocessing import StandardScaler
 
-
 def preprocess(data) :
     data.dropna(inplace=True)
     data.set_index('data_time',inplace=True)
     data.index = pd.to_datetime(data.index)
     data.info()
 
     columns_to_scale = ['ma_q']
@@ -18,86 +18,91 @@
     
     # 스케일링된 열을 포함한 DataFrame 생성
     data_scaled_df = pd.DataFrame(data_scaled, columns=columns_to_scale)
     data_scaled_df = data_scaled_df.set_index(data.index)
     data_scaled_df.rename(columns={'ma_q':'learningma_q'},inplace=True)
     
     # 'ma_Q' 열을 추가하여 원본 DataFrame과 병합
-    data_scaled_df['ma_q'] = data_scaled_df['learningma_q'] # ma_Q/의 경우 scaling 하지 않고 target으로 사용해봄. <=== 해당 부분 문제 가능성이 있어 주석처리
+    data_scaled_df['ma_q'] = data_scaled_df['learningma_q']
     data_scaled_df.drop('learningma_q',axis=1, inplace=True)
 
     features = data_scaled_df.values
     
     return features, scaler2
 
-def correction(data):
+def getLatestDate():
     # 최종학습날짜 확인
     directory = "./example/trainedModels/js/"
     with open(directory+'latest_train_date.txt', 'r' ) as f:
         lines = f.readlines() 
         saved_date = lines[0].strip()
-        
-    df = pd.DataFrame(data)
 
-    cor_df = df[df['data_time'] > str(saved_date)]
+    return str(saved_date)
+
+def correction(data):
+    saved_date = getLatestDate()
+    df = pd.DataFrame(data)
+    df['data_time'] = pd.to_numeric(df['data_time'])
+    cor_df = df[df['data_time'] > int(saved_date)]
     isna = cor_df.isna().sum()
     cols = cor_df.columns
 
     for i in range(len(isna)):
         if isna[i] > 0:
             df[cols[i]].fillna(0, inplace=True)
     
     zeroInd = cor_df[cor_df['ma_q'] == 0]['data_time']
     cor_df['correction'] = 0
     cor_df['ma_pcode'] = '210601'
+    
     if(len(zeroInd) > 0):
         for i in range(len(zeroInd)):
             dt = zeroInd.iloc[i]
-            cor_df.loc[cor_df['data_time'] == dt,'ma_q'] = df.loc[(df.ma_q != 0) & (df.data_time%10000 == zeroInd.iloc[0]%10000)]['ma_q'].mean()
+            cor_df.loc[cor_df['data_time'] == dt,'ma_q'] = df.loc[(df.ma_q != 0) & (df.data_time%10000 == zeroInd.iloc[i]%10000)]['ma_q'].mean()
             cor_df.loc[cor_df['data_time'] == dt, 'correction'] = 1
     
-    insertDB(cor_df)
+    cor_df['data_time'] = cor_df['data_time'].astype('str')
+    insertDB(cor_df, 'flowdata')
     
     cor_df.drop("correction",axis=1, inplace=True)
     cor_df.drop("ma_pcode",axis=1, inplace=True)
-
     result = cor_df.to_dict('records')
 
-    return result
+    cor_df.drop("temp", axis=1, inplace=True)
+    cor_df.drop("humodity", axis=1, inplace=True)
+    cor_df.drop("atmo", axis=1, inplace=True)
+    cor_df.drop("floor", axis=1, inplace=True)
+    cor_df.drop("hr", axis=1, inplace=True)
+    result2 = cor_df.to_dict('records')
+
+    return result, result2
 
 def calStrDate(date):
     list_date = list(date)
-    str_month = int(list_date[5])-1
+    str_month = int(list_date[4]+list_date[5])-1
     if str_month < 1:
         str_month = 12
         list_date[3] = str(int(list_date[3])-1)
-    list_date[5] = str(str_month)
-
+    
+    list_date[4] = str(str_month//10)
+    list_date[5] = str(str_month%10)
+    
     start_date = datetime.strptime(''.join(list_date), "%Y%m%d%H%M")
 
     return start_date
     
 def calEndDate(date, monthVal):
     list_date = list(date)
-    end_month = int(list_date[5])+monthVal
+    end_month = int(list_date[4] + list_date[5])+monthVal
     if end_month > 12:
         end_month -= 12
         list_date[3] = str(int(list_date[3])+1)
         
     list_date[5] = str(end_month)
     end_date = datetime.strptime(''.join(list_date), "%Y%m%d%H%M")
 
     return end_date
 
-def insertDB(df):
-    con = pymysql.connect(host='127.0.0.1', user='root', password='manhattancafe', db='scmsdb011', charset='utf8')
-    cursor = con.cursor()
-    
-    sql = "insert into flowdata (data_time, ma_q, temp, humodity, atmo, floor, hr, correction, ma_pcode) values (%s,%s,%s,%s,%s,%s,%s,%s,%s)"
-    val = df.values.tolist()
-    
-    cursor.excute(sql, val)
-
-    con.commit()
-
-    cursor.close()
-    con.close()
+def insertDB(df, tb_name):
+    engine = create_engine("mysql+pymysql://root:manhattancafe@127.0.0.1:3306/scmsdb011")
+    conn = engine.connect()
+    df.to_sql(name=tb_name, con=engine, if_exists='append', index=False)
```

### Comparing `sswater-0.0.3/sswater/services.py` & `sswater-0.0.4/sswater/services.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,75 +38,78 @@
             self.version = float(lines[1].strip()[1:])
 
         model_list = os.listdir(directory)
         model_list_pt = [file for file in model_list if file.endswith(".pt")]
 
         final_model = directory+model_list_pt[-1]
 
-        self.configs = Config(336,4380,feature_num,False)
+        self.configs = Config(240,2160,feature_num,False)
         if feature_num < 2:
             # 시간 + 유량 모델
             self.model = GAILinear_model(self.configs).cuda()
         else:
             # 추가 데이터 학습 모델
             self.model = NLinear_Model(self.configs).cuda()
         
         # 모델 학습 가중치 .pt 모델 load
         self.model.load_state_dict(torch.load(final_model))
         self.model.eval()
         
 
-    def predict(self,pp_data,scaler,latest_date,input_date,end_date,raw_df,start_date=0):
+    def predict(self,pp_data,scaler,latest_date,input_date,end_date,raw_df,latest_df,start_date=0):
 
         # 전처리 완료 데이터
         last_sequence = pp_data[-self.configs.seq_len:].astype(np.float32)
         # torch 타입으로 변환
         last_sequence = torch.tensor(last_sequence).unsqueeze(0).to(device)
         # 예측 수행
         prediction = self.model(last_sequence).detach().cpu().numpy()
-        
         # 예측 완료 데이터 역정규화
         prediction = scaler.inverse_transform(prediction[:, :, -1])
         
         # input_date보다 크거나 같은 날짜의 유량 데이터 추출 from all data
         totalHour = 0
         input_date = pd.Timestamp(datetime.strptime(str(input_date), "%Y-%m-%d %H:%M:%S"))
 
         if start_date != 0:
             date_str = str(start_date)  # 시작 날짜 및 시간 문자열
             str_date = datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")  # 문자열을 datetime 객체로 변환
             end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
-            totalHour = (end_date - input_date).days * 24 + 24
-            
-            real_ma_Q = raw_df.loc[raw_df.index >= pd.to_datetime(str_date, format='%Y-%m-%d %H:%M'), 'ma_q'].tolist()
+            totalHour = (end_date - input_date).days * 24 - 24
+
+            #print("Month Predict START DATE : ", str_date)
+            temp = raw_df[raw_df.index >= pd.to_datetime(str_date, format='%Y-%m-%d %H:%M')]
+            real_ma_Q = temp.loc[temp.index < input_date, 'ma_q'].tolist()
             total_list = real_ma_Q.copy()
-            
+            input_date = str_date
         else :
             if(end_date != "2300"):
                 end_date = datetime.strptime(str(end_date), "%Y-%m-%d %H:%M:%S")
-                totalHour = (end_date - input_date).days * 24 + 24
+                totalHour = (end_date - input_date).days * 24 - 24
 
             total_list = []
 
-
         prediction_list = prediction[0].tolist()
 
         max_value = raw_df['ma_q'].max()
         min_value = raw_df['ma_q'].min()
         # 예측값 최대 최소
         max_pred = max(prediction_list)
         min_pred = min(prediction_list)
         mean_pred = sum(prediction_list)/len(prediction_list)
+        chLen = len(raw_df[raw_df.index > self.saved_date])
+
+        if(totalHour > 2160):
+                totalHour = 2160
 
         if totalHour > 0:
             for i in range(totalHour):
                 total_list.append(prediction_list[i])
         else :
             for i in range(len(prediction_list)):
                 total_list.append(prediction_list[i])
 
-        #is_real = [1] * len(real_ma_Q) + [0] * len(prediction_list)
         generated_dates = [input_date + timedelta(hours=i) for i in range(0, len(total_list))]
         
-        df = pd.DataFrame({"x": generated_dates, "y": total_list, "last_tr_day": self.saved_date, "last_ver": self.version })
+        df = pd.DataFrame({"x": generated_dates, "y": total_list, "last_tr_day": self.saved_date, "last_ver": self.version, "chlen": chLen, "js": latest_df[0]['js'], "jsb":latest_df[0]['jsb'], "osb":latest_df[0]['osb'], "osbp":latest_df[0]['osbp'] })
 
         return df
```

### Comparing `sswater-0.0.3/sswater/train.py` & `sswater-0.0.4/sswater/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .NLinear import NLinear_Model
 from .GAILinear import GAILinear_model
-
+from .preprocessing import insertDB
 from .create_seq import create_seq
 
 import os
 
 import torch
 import torch.nn.functional as F
 import torch.optim as optim
+import pandas as pd
 from datetime import datetime, timedelta
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 # 학습데이터, 장소, config, 학습특성개수, 추가학습여부
 def model_train(data, place, configs, feature_num, latest_date):
     version = 0 # 첫버전은 0
@@ -36,16 +37,14 @@
         
     with open(directory+'latest_train_date.txt', 'r' ) as f:
         lines = f.readlines()  # 파일의 모든 줄을 읽어옵니다.
 
         # 첫 번째 행의 날짜와 두 번째 행의 버전 값을 분리
         saved_date = lines[0].strip()
         version = float(lines[1].strip()[1:])
-        
-        date_obj = datetime.strptime(lines[0].strip(), "%Y%m%d%H%M").strftime('%Y-%m-%d %H:%M')
 
     X,y =  create_seq(filtered_data, configs.seq_len, configs.pred_len)
     
     # 학습을 위한 설정
     n_epochs = 300
     batch_size = 100
     split_ratio = 0.9
@@ -59,14 +58,15 @@
 
     X_train, y_train = X[:train_samples], y[:train_samples]
     X_val, y_val = X[train_samples:], y[train_samples:]
 
     X_train, X_val = torch.tensor(X_train).float().to(device), torch.tensor(X_val).float().to(device)
     y_train, y_val = torch.tensor(y_train).float().to(device), torch.tensor(y_val).float().to(device)
     
+    print("학습 진행중 ============ ")
     for epoch in range(n_epochs):
         # 모델 학습
         loaded_model.train()
         for i in range(0, X_train.shape[0], batch_size):
             optimizer.zero_grad()
             X_batch = X_train[i:i + batch_size]
             y_batch = y_train[i:i + batch_size]
@@ -76,32 +76,38 @@
             loss.backward()
             optimizer.step()
 
         # 모델 평가
         loaded_model.eval()
         val_output = loaded_model(X_val)
         val_loss = F.mse_loss(val_output, y_val)
-        print(f"Epoch {epoch + 1}, Loss: {loss.item()}, Validation Loss: {val_loss.item()}")
+        #print(f"Epoch {epoch + 1}, Loss: {loss.item()}, Validation Loss: {val_loss.item()}")
     
     # 폴더가 없을시 생성
     try:
         if not os.path.exists(directory):
             os.makedirs(directory)
     except OSError:
         print("Error: Failed to create the directory.")
 
     if version > 0:
         version += 0.1
     else:
         version = 0.1
 
-    file_name = file_name+"_updated_model_"+str(version).replace(".","")+".pt"
-
+    file_name = file_name+"_updated_model.pt"
+    
     if feature_num < 2:
         torch.save(loaded_model.state_dict(), "./example/trainedModels/"+place+"/"+file_name)
     else:
         torch.save(loaded_model.state_dict(), "./example/trainedModels/"+place+"_cli/"+file_name)
     # 업데이트된 날짜와 버전 값을 파일에 기록합니다.
     with open(directory+'latest_train_date.txt', 'w' ) as f:
         f.write(str(latest_date) + '\n') 
         f.write(f'v{version:.1f}')
+    
+    verdf = pd.DataFrame()
+    verdf['version'] = [str(version)]
+    verdf['train_date'] = [str(latest_date)]
+
+    return verdf
```


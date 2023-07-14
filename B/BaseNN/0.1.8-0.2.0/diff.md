# Comparing `tmp/BaseNN-0.1.8.tar.gz` & `tmp/BaseNN-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseNN-0.1.8.tar", last modified: Mon Jul 10 08:35:04 2023, max compression
+gzip compressed data, was "dist/BaseNN-0.2.0.tar", last modified: Fri Jul 14 07:48:09 2023, max compression
```

## Comparing `BaseNN-0.1.8.tar` & `BaseNN-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN/
--rw-rw-r--   0 user      (1001) user      (1001)    39033 2023-07-07 06:54:05.000000 BaseNN-0.1.8/BaseNN/BaseNN.py
--rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.1.8/BaseNN/__init__.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN/examples/
--rw-rw-r--   0 user      (1001) user      (1001)    26768 2023-07-10 08:29:41.000000 BaseNN-0.1.8/BaseNN/examples/BaseNN_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.1.8/BaseNN/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.1.8/BaseNN/examples/pkl2pth.py
--rw-r--r--   0 user      (1001) user      (1001)     4409 2023-05-22 08:15:12.000000 BaseNN-0.1.8/BaseNN/load_data.py
--rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-07-07 06:54:47.000000 BaseNN-0.1.8/BaseNN/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      375 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       80 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-07-10 08:35:04.000000 BaseNN-0.1.8/BaseNN.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.1.8/BaseNN.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-10 08:35:04.000000 BaseNN-0.1.8/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-07-10 08:35:04.000000 BaseNN-0.1.8/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-07-07 06:54:38.000000 BaseNN-0.1.8/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-14 07:48:09.000000 BaseNN-0.2.0/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN/
+-rw-rw-r--   0 user      (1001) user      (1001)    39098 2023-07-14 07:46:38.000000 BaseNN-0.2.0/BaseNN/BaseNN.py
+-rw-rw-r--   0 user      (1001) user      (1001)      270 2023-05-24 09:07:14.000000 BaseNN-0.2.0/BaseNN/__init__.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)    26791 2023-07-13 07:42:58.000000 BaseNN-0.2.0/BaseNN/examples/BaseNN_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-08-26 07:13:38.000000 BaseNN-0.2.0/BaseNN/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-07-11 08:17:06.000000 BaseNN-0.2.0/BaseNN/examples/gradio_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     3059 2023-04-13 07:47:30.000000 BaseNN-0.2.0/BaseNN/examples/pkl2pth.py
+-rw-r--r--   0 user      (1001) user      (1001)     4736 2023-07-13 10:27:43.000000 BaseNN-0.2.0/BaseNN/load_data.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1256 2023-07-14 07:48:01.000000 BaseNN-0.2.0/BaseNN/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      406 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       80 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-07-14 07:48:09.000000 BaseNN-0.2.0/BaseNN.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-18 03:21:26.000000 BaseNN-0.2.0/BaseNN.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)      346 2023-07-14 07:48:09.000000 BaseNN-0.2.0/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-07-14 07:48:09.000000 BaseNN-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     3827 2023-07-12 09:23:07.000000 BaseNN-0.2.0/setup.py
```

### Comparing `BaseNN-0.1.8/BaseNN/BaseNN.py` & `BaseNN-0.2.0/BaseNN/BaseNN.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return x[:, -1, :].unsqueeze(1)
     
 class Squeeze(torch.nn.Module):
     def __init__(self, *args):
         super(Squeeze, self).__init__()
 
     def forward(self, x):
-        return x.squeeze()
+        return x.squeeze(1)
 
 def cal_accuracy(y, pred_y):
     res = pred_y.argmax(axis=1)
     tp = np.array(y.cpu())==np.array(res.cpu())
     acc = np.sum(tp)/ y.shape[0]
     return acc
 
@@ -416,17 +416,20 @@
 
             return self.dataloader
 
     def load_npz_data(self, data_path, batch_size=32, shuffle=True, classes=None,train_val_ratio=1.0):
         from .load_data import NpzDataset
         dataset = NpzDataset(data_path)
         self.dataset_size = int(len(dataset))
-        print(self.dataset_size)
+        # print(self.dataset_size)
         self.img_classes = classes
-        self.word2idx = dataset.word2idx
+        try:
+            self.word2idx = dataset.word2idx
+        except:
+            pass
         # print(self.dataset_size)
         # self.dataloader = DataLoader(dataset,batch_size=batch_size, shuffle=shuffle,num_workers=1)
         if 0 < train_val_ratio < 1:
             train_size =  int(train_val_ratio * self.dataset_size)
             val_size =  self.dataset_size - train_size
 
             train_dataset, val_dataset = torch.utils.data.random_split(dataset, [train_size, val_size])
@@ -781,18 +784,18 @@
                 self. res = res
                 return res
 
             else:  # 推理numpy数组
                 transform = torch.load(checkpoint,map_location=torch.device('cpu'))['meta']['transform']
                 if transform is not None:
                     data = np.array(transform(Image.fromarray(data)))
-                if len(data.shape) == 3:
-                    data = torch.from_numpy(data).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
-                else:
-                    data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
+                # if len(np.array(data).shape) == 3:
+                #     data = torch.from_numpy(data).unsqueeze(0).permute(0,3,1,2).to(torch.float32).to(self.device) 
+                # else:
+                data  = Variable(torch.tensor(np.array(data)).to(torch.float32)).to(self.device)
 
 
             # print(data.shape)
             # data  = Variable(torch.tensor(np.array(data)))
             self.model = self.model.to(self.device)
             self.model.eval()
             with torch.no_grad():
```

### Comparing `BaseNN-0.1.8/BaseNN/examples/BaseNN_demo.py` & `BaseNN-0.2.0/BaseNN/examples/BaseNN_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,14 @@
         print(acc)
         # 训练集准确率：0.9896
         # 验证集准确率：0.9901
     else: # 推理一张图片
         result = model.inference(data=[test_x[0]], checkpoint=checkpoint)
         model.print_result(result)
     
-
 def infer_9_demo():
     model = nn() # 声明模型
     img = cv2.imread("../../111.png",cv2.IMREAD_GRAYSCALE) # 读入测试图片（灰度）
     x = np.expand_dims(img, axis=0) # 增加通道维度
     x = np.expand_dims(x, axis=1) # 增加样本数维度
     # 此时x为四维数组，即[样本数， 通道数，宽， 高]，[1,1,28,28]
     checkpoint = 'mn_ckpt/basenn.pkl'  # 前面训练出的权重文件的路径
@@ -416,22 +415,22 @@
     # print(model.val_label)
 
 def load_npz_data_action():
     # 读取数据
     X = np.load("/home/user/桌面/BaseNN004/BaseNN/examples/human_action_recognition-main/X1.npy",allow_pickle = True)
     y = np.load("/home/user/桌面/BaseNN004/BaseNN/examples/human_action_recognition-main/y1.npy", allow_pickle = True)    
     X = np.load("./conbined.npz")["data"]
-
+    # print(X,X.shape)
     # print(X.shape)
     # np.savez("conbined.npz", data=X, label=y)
     # a = np.load("conbined.npz")
     # print(a['label'].shape)
     # train_x,train_y = X,y.astype(np.float32)
     test_x, test_y = X[28:38,:,:], y[28:38,:].astype(np.float32)
-    # # print(X.shape,train_x.shape, train_y.shape)
+    # print(X.shape,test_x.shape, test_y.shape,test_y)
     # # 搭建模型
     model = nn()
     model.load_npz_data("./conbined.npz",batch_size=50,classes=["a", "b", "c"])
     model.add('lstm', size=(132,128))
     model.add('Dropout',p=0.2)
     model.add('lstm', size=(128,256))
     model.add('Dropout',p=0.2)
@@ -441,15 +440,15 @@
     model.add('BatchNorm1d', size=256)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
     model.add('linear',  size=(256, 256))
     model.add('Linear',  size=(256, 128))
     model.add('linear',  size=(128, 64))
     model.add('Linear',  size=(64, 3))
     model.add(activation='Softmax')
     model.save_fold = "action_ckpt2"
-    model.train(lr=0.01, epochs=10,loss="BCELoss",metrics=[])
+    model.train(lr=0.01, epochs=100,loss="BCELoss",metrics=[])
 
     res = model.inference(test_x, checkpoint="action_ckpt2/basenn.pth")
     print(test_y)
     print(res)
     model.print_result()
 
 def load_npz_data_tang():
@@ -545,21 +544,19 @@
             data.append(verse_l)
         x, y = np.array(data)[:,:-1], np.array(data)[:, 1:]
         print("词表大小：",len(words))
         print("数据集大小：",x.shape[0])
         np.savez(npz_file, data=x, label=y, word2idx=word2idx)
         print("转化成功！保存为：",npz_file)
 
-
 if __name__=="__main__":
     # npz2csv()
     # npz2txt("tang.npz","tangccc.txt")
-
-    txt2npz("tangccc.txt","tangccc_n.npz")
-    # load_npz_data_action()
+    # txt2npz("tangccc.txt","tangccc_n.npz")
+    load_npz_data_action()
     # load_npz_data_tang()
     # tang_infer()
     # txt2npz()
     # action_demo()
     # user_defined_demo()
     # data_define_demo()
     # normal_train_demo()
```

### Comparing `BaseNN-0.1.8/BaseNN/examples/pkl2pth.py` & `BaseNN-0.2.0/BaseNN/examples/pkl2pth.py`

 * *Files identical despite different names*

### Comparing `BaseNN-0.1.8/BaseNN/load_data.py` & `BaseNN-0.2.0/BaseNN/load_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,28 +93,39 @@
 
         return x, y
 
 class NpzDataset(Dataset):
     def __init__(self, root, batch_mode=False):
         self.root = root
         self.batch_mode = batch_mode
-        self.x, self.y = self.load_npz()
+        self.x, self.y,self.word2idx = self.load_npz()
+        # print(self.word2idx)
 
 
     def load_npz(self):
         # x = np.loadtxt(self.root, dtype=float, delimiter=',',skiprows=1) # [120, 4]
         # y = np.loadtxt(self.root, dtype=int, delimiter=',',skiprows=1,usecols=4)
         # data = np.loadtxt(self.root, dtype=float, delimiter=',',skiprows=1) # [120, 4]
-        datas = np.load(self.root)
+        datas = np.load(self.root, allow_pickle=True)
         x = datas["data"]
-        y = datas["label"]
-
-        return x, y
+        y = None
+        word2idx = None
+        try:
+            y = datas["label"]
+        except:
+            pass
+        try:
+            word2idx = datas["word2idx"].item()
+        except:
+            pass
+        return x, y, word2idx
 
     def __len__(self):
-        return self.y.shape[0]
+        return self.x.shape[0]
 
     def __getitem__(self, idx):
         x = torch.tensor(self.x[idx],dtype=torch.float)
-        y = torch.tensor(self.y[idx], dtype=torch.float)
-
+        if self.y is not None:
+            y = torch.tensor(self.y[idx], dtype=torch.float)
+        else:
+            y = None
         return x, y
```

### Comparing `BaseNN-0.1.8/BaseNN/version.py` & `BaseNN-0.2.0/BaseNN/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.8'
+__version__='0.2.0'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseNN-0.1.8/setup.py` & `BaseNN-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     packages = list(gen_packages_items())
     return packages
 
 
 setup(
     name='BaseNN',
-    version='0.1.8',
+    version='0.2.0',
     description='BaseNN can easily build neural networks layer by layer and deeply explore the neural network principle.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```


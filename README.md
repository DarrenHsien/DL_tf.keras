# DL_Level1

## 模組應用區塊
	
### 1.tensorflow.keras.preprocessing.image
	
	-load_img : 讀取影像
	
	-img_to_array : 轉np.array
	
	-ImageDataGenerator : 數據集增強
		-rotation_range : 旋轉角度
		-width_shift_range : 水平平移幅度
		-height_shift_range : 垂直平移幅度
		-shear_range : 以弧度逆时针方向剪切角度
		-zoom_range : 隨機縮放比例
		-horizontal_flip : 水平映射
		-fill_mode : 超出邊界處理
		IDG.flow(image,batch_size= 1 ,save_to_dir=outputPath,save_prefix=prefix,save_format= 'jpg' ) 

### 2.tensorflow.keras.layers
	
	-Conv2D : 二維卷基層(卷積層)
		
		-filter : 輸出過濾器的數目
		-kerbel_size : 卷積核大小
		-strides : 卷積核移動步伐
		-padding : 是否填補0於外圍(valid or same)
		-input_shape : (height , width , depth)
	
	-MaxPooling2D : 最大值精簡矩陣(池化層)
		
		-pool_size : (vertical, horizontal)
		-strides : 移動步伐(默認pool_size)
		-padding : 是否填補0於外圍(valid or same)
		
	-Flatten : 圖像的格式從二維數組（28 x 28像素）轉換為一維數組（28 * 28 = 784像素）該層沒有學習參數。它只會重新格式化數據。
		
		-input_shape : 
		-data_format : 須給定數據為 channels_last channels_first(默認channels_last)

	-Activation : 激活函數
	
	-BatchNormalization : 針對每批上層之激活函數輸出值標準化(中心0標準差1)
		
		-axis : 需歸一化的特徵軸(需參考channels_first(axis = 1) or channels_last(axis = 0))
		
	-Dropout : 










# ORCamera
#### Android 好用的身份证拍照界面封装
<figure class="half">
    <img src="https://upload-images.jianshu.io/upload_images/4179767-d4c4188c4ebd8830.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/400">
    <img src="https://upload-images.jianshu.io/upload_images/4179767-a7097438c43b0954.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/400">
</figure>


`手持身份证`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_GENERAL);
                startActivityForResult(intent, REQUEST_CODE);
```
`身份证正面`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_ID_CARD_FRONT);
                startActivityForResult(intent, REQUEST_CODE);
```
`身份证反面`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_ID_CARD_BACK);
                startActivityForResult(intent, REQUEST_CODE);
```
`CameraActivity.KEY_OUTPUT_FILE_PATH`：拍照后照片要保存的文件
`CameraActivity.KEY_CONTENT_TYPE`：拍照类型
+ CameraActivity.CONTENT_TYPE_GENERAL：手持身份证
+ CameraActivity.CONTENT_TYPE_ID_CARD_FRONT：身份证正面
+ CameraActivity.CONTENT_TYPE_ID_CARD_BACK：身份证反面



`手持身份证`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_GENERAL);
                startActivityForResult(intent, REQUEST_CODE);
```
`身份证正面`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_ID_CARD_FRONT);
                startActivityForResult(intent, REQUEST_CODE);
```
`身份证反面`调用
```java
                Intent intent = new Intent(this, CameraActivity.class);
                intent.putExtra(CameraActivity.KEY_OUTPUT_FILE_PATH,filePath);
                intent.putExtra(CameraActivity.KEY_CONTENT_TYPE, CameraActivity.CONTENT_TYPE_ID_CARD_BACK);
                startActivityForResult(intent, REQUEST_CODE);
```
`CameraActivity.KEY_OUTPUT_FILE_PATH`：拍照后照片要保存的文件
`CameraActivity.KEY_CONTENT_TYPE`：拍照类型
+ CameraActivity.CONTENT_TYPE_GENERAL：手持身份证
+ CameraActivity.CONTENT_TYPE_ID_CARD_FRONT：身份证正面
+ CameraActivity.CONTENT_TYPE_ID_CARD_BACK：身份证反面
+ 剪切图片保存于根目录下cardOrc文件夹内，手持为hand.jpg,身份证正面为:positive.jpg,身份证反面为:reverse.jpg

# 药盒 WebAR 图片追踪 Demo

这个版本先不使用 3D 模型，而是用 OpenCV.js 的 ORB + RANSAC 单应性（Homography）做自然特征追踪：

- `target.jpg`：从你上传的药盒照片中裁出的顶部区域，作为识别目标。
- `ar-content.jpg`：之前上传的彩色烟雾图片，作为 AR 显示内容。
- `index.html`：手机浏览器打开后调用后置摄像头，识别药盒顶部并把图片透视变换到目标表面。

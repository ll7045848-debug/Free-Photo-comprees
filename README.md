<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ImageCompress Pro | Optimize Your Images</title>
    <meta name="description" content="Free online image compression tool. Reduce image file sizes without losing quality. Support for JPG, PNG, and WebP formats.">
    <meta name="keywords" content="image compression, compress images, optimize images, reduce image size, image optimizer">
    <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-YOUR_ADSENSE_ID" crossorigin="anonymous"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #4361ee;
            --primary-dark: #3a0ca3;
            --primary-light: #4895ef;
            --accent: #f72585;
            --secondary: #7209b7;
            --success: #4cc9f0;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --gradient-start: #4361ee;
            --gradient-end: #3a0ca3;
        }
        
        body {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: var(--light);
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.2);
            animation: fadeIn 0.8s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        header {
            background: linear-gradient(135deg, var(--gradient-start), var(--gradient-end));
            color: white;
            padding: 30px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            transform: rotate(30deg);
        }
        
        .logo {
            font-size: 2.8rem;
            font-weight: 800;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            margin-bottom: 10px;
            position: relative;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .logo i {
            color: white;
            font-size: 3.2rem;
            filter: drop-shadow(0 2px 5px rgba(0, 0, 0, 0.3));
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            margin-bottom: 10px;
            position: relative;
        }
        
        .stats {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
            position: relative;
        }
        
        .stat-item {
            text-align: center;
        }
        
        .stat-number {
            font-size: 2.2rem;
            font-weight: 700;
            color: white;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        
        .stat-label {
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .content {
            display: grid;
            grid-template-columns: 1fr 350px;
            gap: 25px;
            padding: 30px;
        }
        
        @media (max-width: 900px) {
            .content {
                grid-template-columns: 1fr;
            }
        }
        
        .main-content {
            flex: 1;
        }
        
        .compression-tool {
            background: rgba(255, 255, 255, 0.08);
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s;
        }
        
        .compression-tool:hover {
            transform: translateY(-5px);
        }
        
        h2 {
            color: white;
            margin-bottom: 20px;
            font-size: 2rem;
            font-weight: 700;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            position: relative;
            display: inline-block;
        }
        
        h2::after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -8px;
            width: 50px;
            height: 4px;
            background: var(--accent);
            border-radius: 2px;
        }
        
        .upload-area {
            border: 3px dashed rgba(255, 255, 255, 0.3);
            border-radius: 15px;
            padding: 50px 30px;
            text-align: center;
            margin-bottom: 25px;
            cursor: pointer;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .upload-area:hover {
            border-color: rgba(255, 255, 255, 0.5);
            background: rgba(255, 255, 255, 0.05);
        }
        
        .upload-area.active {
            border-color: var(--success);
            background: rgba(76, 201, 240, 0.1);
        }
        
        .upload-icon {
            font-size: 4.5rem;
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 20px;
            transition: all 0.3s;
        }
        
        .upload-area:hover .upload-icon {
            color: white;
            transform: scale(1.1);
        }
        
        .upload-text {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }
        
        .upload-subtext {
            font-size: 0.9rem;
            opacity: 0.7;
        }
        
        .file-input {
            display: none;
        }
        
        .compression-controls {
            margin: 30px 0;
        }
        
        .control-group {
            margin-bottom: 25px;
            background: rgba(255, 255, 255, 0.05);
            padding: 20px;
            border-radius: 12px;
        }
        
        .slider-container {
            margin-bottom: 20px;
        }
        
        .slider-label {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
        }
        
        .slider-value {
            font-weight: 700;
            color: var(--success);
            font-size: 1.2rem;
        }
        
        .slider {
            width: 100%;
            height: 12px;
            -webkit-appearance: none;
            appearance: none;
            background: linear-gradient(to right, #4cc9f0, #4361ee, #3a0ca3);
            outline: none;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        
        .slider::-webkit-slider-thumb {
            -webkit-appearance: none;
            appearance: none;
            width: 28px;
            height: 28px;
            border-radius: 50%;
            background: white;
            cursor: pointer;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
            border: 2px solid var(--primary);
            transition: all 0.2s;
        }
        
        .slider::-webkit-slider-thumb:hover {
            transform: scale(1.1);
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.4);
        }
        
        .slider-labels {
            display: flex;
            justify-content: space-between;
            margin-top: 10px;
            color: rgba(255, 255, 255, 0.7);
            font-size: 0.9rem;
        }
        
        .format-selection {
            display: flex;
            gap: 15px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .format-btn {
            padding: 12px 25px;
            background: rgba(255, 255, 255, 0.1);
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 8px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
            color: rgba(255, 255, 255, 0.8);
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .format-btn.active {
            background: var(--primary);
            color: white;
            border-color: var(--primary-light);
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.3);
        }
        
        .format-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .action-btn {
            display: block;
            width: 100%;
            padding: 18px;
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            border: none;
            border-radius: 10px;
            font-size: 1.2rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s;
            margin: 30px 0;
            box-shadow: 0 5px 15px rgba(67, 97, 238, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .action-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: all 0.5s;
        }
        
        .action-btn:hover::before {
            left: 100%;
        }
        
        .action-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(67, 97, 238, 0.4);
        }
        
        .action-btn:active {
            transform: translateY(0);
        }
        
        .results {
            display: none;
            background: rgba(255, 255, 255, 0.08);
            border-radius: 15px;
            padding: 30px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.1);
            margin-top: 30px;
            animation: fadeIn 0.5s ease-out;
        }
        
        .comparison {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
            margin: 25px 0;
        }
        
        @media (max-width: 600px) {
            .comparison {
                grid-template-columns: 1fr;
            }
        }
        
        .image-box {
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            padding: 20px;
            background: rgba(255, 255, 255, 0.05);
            transition: transform 0.3s;
        }
        
        .image-box:hover {
            transform: translateY(-5px);
        }
        
        .image-box h4 {
            margin-bottom: 15px;
            font-size: 1.2rem;
            color: white;
        }
        
        .image-box img {
            max-width: 100%;
            max-height: 250px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .image-info {
            margin-top: 15px;
            color: rgba(255, 255, 255, 0.8);
            font-size: 0.9rem;
        }
        
        .savings {
            text-align: center;
            padding: 20px;
            background: rgba(76, 201, 240, 0.1);
            border-radius: 12px;
            margin: 25px 0;
            color: white;
            border: 1px solid rgba(76, 201, 240, 0.3);
        }
        
        .savings h4 {
            margin-bottom: 10px;
            font-size: 1.2rem;
        }
        
        .savings-percent {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--success);
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        
        .download-btn {
            display: inline-block;
            padding: 15px 35px;
            background: linear-gradient(135deg, var(--success), #3aa5c9);
            color: white;
            text-decoration: none;
            border-radius: 10px;
            font-weight: 700;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(76, 201, 240, 0.3);
        }
        
        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(76, 201, 240, 0.4);
        }
        
        .download-btn:active {
            transform: translateY(0);
        }
        
        .center {
            text-align: center;
            margin: 20px 0;
        }
        
        .sidebar {
            background: rgba(255, 255, 255, 0.08);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .ad-container {
            margin-bottom: 25px;
            text-align: center;
            border: 2px dashed rgba(255, 255, 255, 0.2);
            border-radius: 12px;
            padding: 25px;
            background: rgba(255, 255, 255, 0.05);
            min-height: 280px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }
        
        .ad-label {
            display: block;
            text-align: center;
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.8rem;
            margin-bottom: 10px;
            text-transform: uppercase;
        }
        
        .ad-placeholder {
            width: 100%;
            height: 250px;
            background: linear-gradient(135deg, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0.05));
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(255, 255, 255, 0.5);
            font-size: 0.9rem;
        }
        
        .tips {
            margin-top: 30px;
        }
        
        .tips h3 {
            color: white;
            margin-bottom: 15px;
            font-size: 1.3rem;
        }
        
        .tips ul {
            list-style: none;
        }
        
        .tips li {
            margin-bottom: 12px;
            padding-left: 25px;
            position: relative;
            color: rgba(255, 255, 255, 0.8);
        }
        
        .tips li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: 700;
        }
        
        footer {
            text-align: center;
            padding: 30px;
            background: rgba(0, 0, 0, 0.2);
            margin-top: 40px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            gap: 25px;
            margin: 20px 0;
            flex-wrap: wrap;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        /* Ad spaces in content */
        .ad-in-content {
            margin: 40px 0;
            text-align: center;
        }
        
        .ad-wide {
            width: 100%;
            min-height: 90px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 12px;
            display: flex;
            justify-content: center;
            align-items: center;
            border: 2px dashed rgba(255, 255, 255, 0.2);
            margin: 30px 0;
        }
        
        /* Responsive ads */
        @media (max-width: 768px) {
            .ad-container {
                min-height: 200px;
            }
            
            .ad-placeholder {
                height: 150px;
            }
            
            .ad-wide {
                min-height: 70px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">
                <i class="fas fa-compress-alt"></i>
                <span>ImageCompress Pro</span>
            </div>
            <p class="tagline">Optimize your images without losing quality</p>
            
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">87%</div>
                    <div class="stat-label">Average Savings</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">5.2M+</div>
                    <div class="stat-label">Images Compressed</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">0.1s</div>
                    <div class="stat-label">Avg. Processing Time</div>
                </div>
            </div>
        </header>
        
        <div class="content">
            <div class="main-content">
                <!-- Top Ad Banner -->
                <div class="ad-in-content">
                    <div class="ad-label">Advertisement</div>
                    <div class="ad-wide">
                        <!-- AdSense Ad Unit for Banner -->
                        <ins class="adsbygoogle"
                             style="display:block"
                             data-ad-client="<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-3196265639258501"
     crossorigin="anonymous"></script>"
                             data-ad-slot="<script async custom-element="amp-auto-ads"
        src="https://cdn.ampproject.org/v0/amp-auto-ads-0.1.js">
</script>"
                             data-ad-format="auto"
                             data-full-width-responsive="true"></ins>
                        <script>
                             (adsbygoogle = window.adsbygoogle || []).push({});
                        </script>
                    </div>
                </div>
                
                <div class="compression-tool">
                    <h2>Image Compression Tool</h2>
                    <p>Reduce image file size without sacrificing quality. Supports JPG, PNG, and WebP formats.</p>
                    
                    <div class="upload-area" id="uploadArea">
                        <div class="upload-icon">
                            <i class="fas fa-cloud-upload-alt"></i>
                        </div>
                        <p class="upload-text">Drag & drop your image here or click to browse</p>
                        <p class="upload-subtext">Max file size: 5MB • JPG, PNG, WebP</p>
                        <input type="file" id="fileInput" class="file-input" accept="image/*">
                    </div>
                    
                    <div class="compression-controls">
                        <div class="control-group">
                            <h3>Compression Settings</h3>
                            
                            <div class="slider-container">
                                <div class="slider-label">
                                    <span>Compression Level</span>
                                    <span class="slider-value" id="compressionValue">70%</span>
                                </div>
                                <input type="range" id="compressionLevel" class="slider" min="0" max="100" value="70">
                                <div class="slider-labels">
                                    <span>Smaller File</span>
                                    <span>Better Quality</span>
                                </div>
                            </div>
                            
                            <div class="format-selection">
                                <label>Output Format:</label>
                                <button class="format-btn active" data-format="jpeg">
                                    <i class="fas fa-file-image"></i> JPEG
                                </button>
                                <button class="format-btn" data-format="png">
                                    <i class="fas fa-file-image"></i> PNG
                                </button>
                                <button class="format-btn" data-format="webp">
                                    <i class="fas fa-file-image"></i> WebP
                                </button>
                            </div>
                        </div>
                    </div>
                    
                    <button id="compressBtn" class="action-btn">
                        <i class="fas fa-bolt"></i> Compress Image
                    </button>
                    
                    <div id="results" class="results">
                        <h2>Compression Results</h2>
                        
                        <div class="comparison">
                            <div class="image-box">
                                <h4>Original Image</h4>
                                <img id="originalImg" src="" alt="Original image">
                                <div class="image-info">
                                    Size: <span id="originalSize">0 KB</span>
                                </div>
                            </div>
                            <div class="image-box">
                                <h4>Compressed Image</h4>
                                <img id="compressedImg" src="" alt="Compressed image">
                                <div class="image-info">
                                    Size: <span id="compressedSize">0 KB</span>
                                </div>
                            </div>
                        </div>
                        
                        <div class="savings">
                            <h4>You saved</h4>
                            <div class="savings-percent" id="savingsPercent">0%</div>
                            <p>of the original file size!</p>
                        </div>
                        
                        <div class="center">
                            <a href="#" id="downloadBtn" class="download-btn">
                                <i class="fas fa-download"></i> Download Compressed Image
                            </a>
                        </div>
                    </div>
                </div>
                
                <!-- Middle Ad Banner -->
                <div class="ad-in-content">
                    <div class="ad-label">Advertisement</div>
                    <div class="ad-wide">
                        <!-- AdSense Ad Unit for Banner -->
                        <ins class="adsbygoogle"
                             style="display:block"
                             data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                             data-ad-slot="YOUR_BANNER_SLOT_ID"
                             data-ad-format="auto"
                             data-full-width-responsive="true"></ins>
                        <script>
                             (adsbygoogle = window.adsbygoogle || []).push({});
                        </script>
                    </div>
                </div>
            </div>
            
            <div class="sidebar">
                <div class="ad-container">
                    <span class="ad-label">Advertisement</span>
                    <div class="ad-placeholder">
                        <!-- AdSense Ad Unit for Square -->
                        <ins class="adsbygoogle"
                             style="display:block"
                             data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                             data-ad-slot="YOUR_SQUARE_SLOT_ID"
                             data-ad-format="auto"
                             data-full-width-responsive="true"></ins>
                        <script>
                             (adsbygoogle = window.adsbygoogle || []).push({});
                        </script>
                    </div>
                </div>
                
                <div class="ad-container">
                    <span class="ad-label">Advertisement</span>
                    <div class="ad-placeholder">
                        <!-- AdSense Ad Unit for Rectangle -->
                        <ins class="adsbygoogle"
                             style="display:block"
                             data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                             data-ad-slot="YOUR_RECTANGLE_SLOT_ID"
                             data-ad-format="auto"
                             data-full-width-responsive="true"></ins>
                        <script>
                             (adsbygoogle = window.adsbygoogle || []).push({});
                        </script>
                    </div>
                </div>
                
                <div class="tips">
                    <h3>Image Optimization Tips</h3>
                    <ul>
                        <li>Use WebP format for better compression</li>
                        <li>Choose the right compression level for your needs</li>
                        <li>Resize images before uploading for better results</li>
                        <li>Use appropriate dimensions for your website</li>
                        <li>Compress images before sending via email</li>
                    </ul>
                </div>
            </div>
        </div>
        
        <!-- Bottom Ad Banner -->
        <div class="ad-in-content">
            <div class="ad-label">Advertisement</div>
            <div class="ad-wide">
                <!-- AdSense Ad Unit for Banner -->
                <ins class="adsbygoogle"
                     style="display:block"
                     data-ad-client="ca-pub-YOUR_ADSENSE_ID"
                     data-ad-slot="YOUR_BANNER_SLOT_ID"
                     data-ad-format="auto"
                     data-full-width-responsive="true"></ins>
                <script>
                     (adsbygoogle = window.adsbygoogle || []).push({});
                </script>
            </div>
        </div>
        
        <footer>
            <p>&copy; 2023 ImageCompress Pro. All rights reserved.</p>
            <div class="footer-links">
                <a href="#">Privacy Policy</a>
                <a href="#">Terms of Service</a>
                <a href="#">Contact Us</a>
                <a href="#">API Documentation</a>
                <a href="#">Help Center</a>
            </div>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const fileInput = document.getElementById('fileInput');
            const uploadArea = document.getElementById('uploadArea');
            const compressionLevel = document.getElementById('compressionLevel');
            const compressionValue = document.getElementById('compressionValue');
            const compressBtn = document.getElementById('compressBtn');
            const results = document.getElementById('results');
            const originalImg = document.getElementById('originalImg');
            const compressedImg = document.getElementById('compressedImg');
            const originalSize = document.getElementById('originalSize');
            const compressedSize = document.getElementById('compressedSize');
            const savingsPercent = document.getElementById('savingsPercent');
            const downloadBtn = document.getElementById('downloadBtn');
            const formatButtons = document.querySelectorAll('.format-btn');
            
            let currentFile = null;
            let currentFormat = 'jpeg';
            
            // Update compression value display
            compressionLevel.addEventListener('input', function() {
                compressionValue.textContent = `${this.value}%`;
            });
            
            // Format selection
            formatButtons.forEach(button => {
                button.addEventListener('click', function() {
                    formatButtons.forEach(btn => btn.classList.remove('active'));
                    this.classList.add('active');
                    currentFormat = this.getAttribute('data-format');
                });
            });
            
            // Upload area functionality
            uploadArea.addEventListener('click', function() {
                fileInput.click();
            });
            
            uploadArea.addEventListener('dragover', function(e) {
                e.preventDefault();
                this.classList.add('active');
            });
            
            uploadArea.addEventListener('dragleave', function() {
                this.classList.remove('active');
            });
            
            uploadArea.addEventListener('drop', function(e) {
                e.preventDefault();
                this.classList.remove('active');
                
                if (e.dataTransfer.files.length) {
                    handleFile(e.dataTransfer.files[0]);
                }
            });
            
            fileInput.addEventListener('change', function() {
                if (this.files.length) {
                    handleFile(this.files[0]);
                }
            });
            
            // Handle the selected file
            function handleFile(file) {
                if (!file.type.match('image.*')) {
                    alert('Please select an image file.');
                    return;
                }
                
                if (file.size > 5 * 1024 * 1024) {
                    alert('File size exceeds 5MB limit.');
                    return;
                }
                
                currentFile = file;
                uploadArea.classList.add('active');
                
                const reader = new FileReader();
                reader.onload = function(e) {
                    originalImg.src = e.target.result;
                    originalSize.textContent = formatBytes(file.size);
                    
                    // Reset results
                    results.style.display = 'none';
                };
                reader.readAsDataURL(file);
            }
            
            // Compress image
            compressBtn.addEventListener('click', function() {
                if (!currentFile) {
                    alert('Please select an image first.');
                    return;
                }
                
                // Show compressing animation
                this.classList.add('compressing');
                this.innerHTML = '<i class="fas fa-cog fa-spin"></i> Compressing...';
                
                setTimeout(function() {
                    const quality = compressionLevel.value / 100;
                    
                    const reader = new FileReader();
                    reader.onload = function(e) {
                        const img = new Image();
                        img.onload = function() {
                            const canvas = document.createElement('canvas');
                            const ctx = canvas.getContext('2d');
                            
                            // Calculate new dimensions if needed
                            let width = img.width;
                            let height = img.height;
                            
                            // Set canvas dimensions
                            canvas.width = width;
                            canvas.height = height;
                            
                            // Draw image on canvas
                            ctx.drawImage(img, 0, 0, width, height);
                            
                            // Get compressed data URL
                            let compressedDataURL;
                            switch (currentFormat) {
                                case 'jpeg':
                                    compressedDataURL = canvas.toDataURL('image/jpeg', quality);
                                    break;
                                case 'png':
                                    compressedDataURL = canvas.toDataURL('image/png');
                                    break;
                                case 'webp':
                                    compressedDataURL = canvas.toDataURL('image/webp', quality);
                                    break;
                            }
                            
                            // Display compressed image
                            compressedImg.src = compressedDataURL;
                            
                            // Calculate sizes
                            const originalSizeBytes = currentFile.size;
                            const compressedSizeBytes = Math.round((compressedDataURL.length * 3) / 4);
                            
                            originalSize.textContent = formatBytes(originalSizeBytes);
                            compressedSize.textContent = formatBytes(compressedSizeBytes);
                            
                            // Calculate savings
                            const savings = 100 - Math.round((compressedSizeBytes / originalSizeBytes) * 100);
                            savingsPercent.textContent = savings + '%';
                            
                            // Set download link
                            downloadBtn.href = compressedDataURL;
                            downloadBtn.download = 'compressed-image.' + currentFormat;
                            
                            // Show results
                            results.style.display = 'block';
                            
                            // Reset button
                            compressBtn.classList.remove('compressing');
                            compressBtn.innerHTML = '<i class="fas fa-bolt"></i> Compress Image';
                        };
                        img.src = e.target.result;
                    };
                    reader.readAsDataURL(currentFile);
                }, 1000); // Simulate processing time
            });
            
            // Format bytes to readable format
            function formatBytes(bytes, decimals = 2) {
                if (bytes === 0) return '0 Bytes';
                
                const k = 1024;
                const dm = decimals < 0 ? 0 : decimals;
                const sizes = ['Bytes', 'KB', 'MB', 'GB'];
                
                const i = Math.floor(Math.log(bytes) / Math.log(k));
                
                return parseFloat((bytes / Math.pow(k, i)).toFixed(dm)) + ' ' + sizes[i];
            }
        });
    </script>
</body>
</html>

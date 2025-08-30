# 
<!DOCTYPE html>
<html lang="en">
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIK Studio - Perfect Tablet Builder</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/three@0.128.0/examples/js/controls/OrbitControls.js"></script>
</head>
<body>
    <div class="container">
        <header>
            <h1>🚀 VIK Studio</h1>
            <p>Perfect Tablet Builder For 3D & JC</p>
        </header>
        
        <div class="builder-interface">
            <div class="controls-panel">
                <h2>📱 Customize Your Tablet</h2>
                
                <div class="control-group">
                    <label for="screen-size">Screen Size:</label>
                    <select id="screen-size">
                        <option value="8">8 inch</option>
                        <option value="10" selected>10 inch</option>
                        <option value="12">12 inch</option>
                        <option value="15">15 inch</option>
                    </select>
                </div>
                
                <div class="control-group">
                    <label for="color">Color:</label>
                    <select id="color">
                        <option value="#2c3e50">Space Gray</option>
                        <option value="#ecf0f1" selected>Silver</option>
                        <option value="#e74c3c">Red</option>
                        <option value="#3498db">Blue</option>
                        <option value="#27ae60">Green</option>
                        <option value="#000000">Black</option>
                    </select>
                </div>
                
                <div class="control-group">
                    <label for="storage">Storage:</label>
                    <select id="storage">
                        <option value="64">64 GB</option>
                        <option value="128" selected>128 GB</option>
                        <option value="256">256 GB</option>
                        <option value="512">512 GB</option>
                        <option value="1024">1 TB</option>
                    </select>
                </div>
                
                <div class="control-group">
                    <label for="ram">RAM:</label>
                    <select id="ram">
                        <option value="4">4 GB</option>
                        <option value="8" selected>8 GB</option>
                        <option value="16">16 GB</option>
                        <option value="32">32 GB</option>
                    </select>
                </div>
                
                <div class="control-group">
                    <label for="processor">Processor:</label>
                    <select id="processor">
                        <option value="A15">A15 Bionic</option>
                        <option value="M1" selected>M1 Chip</option>
                        <option value="M2">M2 Chip</option>
                        <option value="Snapdragon">Snapdragon 8 Gen 2</option>
                    </select>
                </div>
                
                <div class="control-group">
                    <label>
                        <input type="checkbox" id="cellular"> 📶 Cellular
                    </label>
                </div>
                
                <div class="control-group">
                    <label>
                        <input type="checkbox" id="stylus" checked> ✏️ Stylus Support
                    </label>
                </div>
                
                <div class="price-display">
                    <h3>💰 Price: $<span id="price">899</span></h3>
                </div>
                
                <button id="build-tablet" class="build-btn">🎯 Build My Tablet</button>
            </div>
            
            <div class="preview-panel">
                <h2>🎨 3D Preview</h2>
                <div id="tablet-preview"></div>
                <div class="preview-controls">
                    <button id="rotate-left">↺ Rotate Left</button>
                    <button id="rotate-right">↻ Rotate Right</button>
                    <button id="reset-view">🎯 Reset View</button>
                </div>
            </div>
        </div>
        
        <div class="specs-display" id="specs-display" style="display: none;">
            <h2>📋 Your Custom Tablet Specs</h2>
            <div id="final-specs"></div>
            <button id="export-config">💾 Export Configuration</button>
            <button id="new-build">🔄 Build Another</button>
        </div>
    </div>
    
    <script src="script.js"></script>
</body>
</html>

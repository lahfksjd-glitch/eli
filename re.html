<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>社會住宅包租代管 修繕補助送件表</title>
    <!-- 引入 html2pdf.js 解決行動裝置/iPad 列印跑版問題 -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
    <style>
        :root {
            --border-color: #000000;
            --text-color: #000000;
            --btn-primary: #1a365d;
            --btn-secondary: #2b6cb0;
        }

        * {
            box-sizing: border-box;
        }

        /* 全域指定標楷體、字體大小 14pt */
        body, input, textarea, select, button, table, td, th {
            font-family: "標楷體", "BiauKai", "DFKai-SB", "TW-Kai", serif !important;
            font-size: 14pt !important;
            color: var(--text-color);
        }

        body {
            margin: 0;
            padding: 15px;
            background-color: #f0f4f8;
            -webkit-text-size-adjust: 100%;
        }

        .wrapper {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
        }

        /* 頂部操作按鈕 */
        .action-bar {
            position: fixed;
            top: 15px;
            right: 25px;
            display: flex;
            gap: 8px;
            z-index: 100;
        }

        .btn-export {
            background-color: var(--btn-primary);
            color: #ffffff !important;
            border: none;
            padding: 8px 18px;
            border-radius: 4px;
            cursor: pointer;
            font-weight: bold;
            box-shadow: 0 2px 8px rgba(0,0,0,0.25);
            transition: all 0.2s;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .btn-export:hover {
            background-color: var(--btn-secondary);
        }

        /* 單頁 A4 規格卡片（邊界 12.7mm 約 0.5 英吋） */
        .page-sheet {
            background-color: #ffffff;
            padding: 24px 28px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            margin-bottom: 24px;
            position: relative;
            min-height: 1100px;
        }

        /* 第一頁強制分頁 */
        .page-sheet.page-1 {
            page-break-after: always !important;
            break-after: page !important;
        }

        /* 表格基礎排版 */
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 12px;
            table-layout: fixed;
        }

        th, td {
            padding: 6px 8px;
            vertical-align: middle;
        }

        /* ========== 頁首物件資料：完全不顯示格線 ========== */
        .header-table {
            border: none !important;
            margin-bottom: 16px;
        }

        .header-table td {
            border: none !important;
            font-weight: bold;
            padding: 4px 4px;
        }

        input[type="text"], textarea {
            width: 100%;
            border: none;
            outline: none;
            background: transparent;
            padding: 2px 4px;
            box-sizing: border-box;
            font-weight: bold;
        }

        input[type="text"]:focus, textarea:focus {
            background-color: #fffdf0;
        }

        /* ========== 第一頁：照片固定寬 18cm、高 15cm，滿版無黑邊 ========== */
        .p1-photo-row {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            margin-bottom: 18px;
        }

        .p1-dropzone {
            width: 18cm;
            height: 15cm;
            max-width: 100%;
            border: 1.5px dashed #cbd5e0;
            border-radius: 4px;
            background-color: #ffffff;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            overflow: hidden;
            position: relative;
        }

        .p1-dropzone:hover {
            border-color: #718096;
            background-color: #f7fafc;
        }

        .p1-dropzone img {
            width: 100%;
            height: 100%;
            display: none;
            object-fit: cover; /* 自動符合寬高，完全去除黑邊 */
            background-color: #ffffff;
        }

        .dropzone-tip {
            color: #718096;
            font-weight: bold;
            pointer-events: none;
            padding: 10px;
            text-align: center;
        }

        .hidden-file-input {
            display: none;
        }

        /* ========== 第二頁：修繕對照表（保留表格線條） ========== */
        .compare-table {
            border: 1px solid var(--border-color);
        }

        .compare-table td, .compare-table th {
            border: 1px solid var(--border-color);
        }

        .compare-table td.col-label {
            width: 14%;
            text-align: center;
            font-weight: bold;
            letter-spacing: 2px;
        }

        .compare-table td.col-content {
            width: 86%;
            padding: 8px;
        }

        .remarks-container {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .remarks-select-row {
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .remarks-select {
            flex: 1;
            padding: 4px 6px;
            border: 1px solid #cbd5e0;
            border-radius: 4px;
            background-color: #f8fafc;
            color: #2d3748;
            cursor: pointer;
        }

        .remarks-select:focus {
            border-color: var(--btn-secondary);
            outline: none;
            background-color: #ffffff;
        }

        .btn-clear-note {
            background-color: #edf2f7;
            color: #4a5568;
            border: 1px solid #cbd5e0;
            padding: 4px 10px;
            border-radius: 4px;
            cursor: pointer;
            white-space: nowrap;
        }

        .btn-clear-note:hover {
            background-color: #e2e8f0;
            color: #e53e3e;
        }

        textarea.remarks-input {
            width: 100%;
            min-height: 54px;
            padding: 6px 8px;
            border: 1px solid #e2e8f0;
            border-radius: 4px;
            background-color: #ffffff;
            line-height: 1.5;
            resize: vertical;
        }

        textarea.remarks-input:focus {
            border-color: var(--btn-secondary);
            background-color: #fffdf0;
        }

        /* ========== 第二頁：照片固定寬 8cm、高 8.5cm（無黑邊，滿版裁切） ========== */
        .multi-photo-wrapper {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .btn-add-photos {
            align-self: flex-start;
            background-color: #edf2f7;
            color: var(--btn-secondary);
            border: 1px dashed #cbd5e0;
            padding: 4px 10px;
            border-radius: 4px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.2s;
        }

        .btn-add-photos:hover {
            background-color: #e2e8f0;
            border-color: var(--btn-secondary);
        }

        .photo-gallery-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            align-items: center;
        }

        .photo-thumb-card {
            position: relative;
            width: 8cm;
            height: 8.5cm;
            border: 1px solid #cbd5e0;
            background-color: #ffffff;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            border-radius: 4px;
        }

        .photo-thumb-card img {
            width: 100%;
            height: 100%;
            object-fit: cover; /* 自動符合寬高，完全去除黑邊 */
        }

        .photo-thumb-del {
            position: absolute;
            top: 4px;
            right: 4px;
            background: rgba(229, 62, 62, 0.9);
            color: #ffffff;
            border: none;
            border-radius: 50%;
            width: 24px;
            height: 24px;
            font-size: 12pt !important;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 5;
        }

        .photo-thumb-del:hover {
            background: #c53030;
        }

        .empty-photo-tip {
            color: #a0aec0;
            padding: 10px;
            border: 1px dashed #e2e8f0;
            border-radius: 4px;
            width: 100%;
            text-align: center;
        }

        /* ========== A4 列印與 PDF 匯出規則 ========== */
        @page {
            size: A4 portrait;
            margin: 12.7mm;
        }

        @media print {
            body {
                background: white;
                padding: 0;
                margin: 0;
            }
            .wrapper {
                max-width: 100% !important;
            }
            .page-sheet {
                box-shadow: none !important;
                padding: 0 !important;
                margin: 0 !important;
                min-height: auto !important;
            }
            .page-sheet.page-1 {
                page-break-after: always !important;
                break-after: page !important;
            }
            .action-bar, .dropzone-tip, .remarks-select-row, .btn-add-photos, .photo-thumb-del, .empty-photo-tip {
                display: none !important;
            }
            .p1-dropzone {
                border: none !important;
                width: 18cm !important;
                height: 15cm !important;
                max-width: 100% !important;
                background: transparent !important;
            }
            .header-table, .header-table td {
                border: none !important;
            }
            textarea.remarks-input {
                border: none !important;
                background: transparent !important;
                padding: 0 !important;
                resize: none !important;
            }
            table, tr, td {
                page-break-inside: avoid;
                break-inside: avoid;
            }
            .photo-thumb-card {
                width: 8cm !important;
                height: 8.5cm !important;
                border: 1px solid #000000 !important;
            }
        }

        /* html2pdf 渲染樣式 */
        .rendering-pdf {
            width: 100% !important;
            max-width: 100% !important;
            padding: 0 !important;
            box-shadow: none !important;
        }
        .rendering-pdf .page-sheet {
            box-shadow: none !important;
            padding: 10px 0 !important;
            margin: 0 !important;
            min-height: auto !important;
        }
        .rendering-pdf .page-sheet.page-1 {
            page-break-after: always !important;
            break-after: page !important;
        }
        .rendering-pdf .action-bar,
        .rendering-pdf .dropzone-tip,
        .rendering-pdf .remarks-select-row,
        .rendering-pdf .btn-add-photos,
        .rendering-pdf .photo-thumb-del,
        .rendering-pdf .empty-photo-tip {
            display: none !important;
        }
        .rendering-pdf .p1-dropzone {
            border: none !important;
            width: 18cm !important;
            height: 15cm !important;
            max-width: 100% !important;
            background: transparent !important;
        }
        .rendering-pdf .header-table,
        .rendering-pdf .header-table td {
            border: none !important;
        }
        .rendering-pdf textarea.remarks-input {
            border: none !important;
            background: transparent !important;
            padding: 0 !important;
            resize: none !important;
        }
        .rendering-pdf table,
        .rendering-pdf tr,
        .rendering-pdf td {
            page-break-inside: avoid;
            break-inside: avoid;
        }
        .rendering-pdf .photo-thumb-card {
            width: 8cm !important;
            height: 8.5cm !important;
            border: 1px solid #000000 !important;
        }
    </style>
</head>
<body>

<div class="action-bar">
    <button type="button" class="btn-export" onclick="exportToPDF()">
        📥 匯出送件 PDF (完整雙頁)
    </button>
</div>

<div class="wrapper" id="pdf-export-root">
    <!-- ==================== 第一頁 (單據與工單) ==================== -->
    <div class="page-sheet page-1">
        <!-- 頁首物件基本資訊表（無框線） -->
        <table class="header-table">
            <colgroup>
                <col style="width: 15%;">
                <col style="width: 29%;">
                <col style="width: 15%;">
                <col style="width: 41%;">
            </colgroup>
            <tr>
                <td style="text-align: center;">物件編號</td>
                <td><input type="text" class="sync-prop-id" placeholder="" oninput="syncFields('prop-id', this.value)"></td>
                <td style="text-align: right;">房東姓名</td>
                <td><input type="text" class="sync-landlord" value="" oninput="syncFields('landlord', this.value)"></td>
            </tr>
            <tr>
                <td style="text-align: center;">媒合編號</td>
                <td><input type="text" class="sync-match-id" placeholder="" oninput="syncFields('match-id', this.value)"></td>
                <td style="text-align: right;">物件地址</td>
                <td><input type="text" class="sync-address" value="" oninput="syncFields('address', this.value)"></td>
            </tr>
            <tr>
                <td style="text-align: center;">租賃期間</td>
                <td colspan="3">
                    <input type="text" class="sync-lease" value="115/11/01 ~ 116/10/31" oninput="syncFields('lease', this.value)">
                </td>
            </tr>
        </table>

        <!-- 發票 / 購買憑證截圖  -->
        <div class="p1-photo-row">
            <input type="file" id="invoice-file" class="hidden-file-input" accept="image/*" onchange="previewP1Image(this, 'invoice-img', 'invoice-tip')">
            <div class="p1-dropzone" onclick="document.getElementById('invoice-file').click()" title="點擊上傳或更換發票截圖 (寬18cm 高15cm)">
                <span class="dropzone-tip" id="invoice-tip">📷 點擊上傳「發票 / 電子發票明細截圖」<br>(寬 18cm × 高 15cm)</span>
                <img id="invoice-img" alt="發票截圖">
            </div>
        </div>

        <!-- 廠商施工服務單 / 維修工單  -->
        <div class="p1-photo-row">
            <input type="file" id="receipt-file" class="hidden-file-input" accept="image/*" onchange="previewP1Image(this, 'receipt-img', 'receipt-tip')">
            <div class="p1-dropzone" onclick="document.getElementById('receipt-file').click()" title="點擊上傳或更換廠商工單 (寬18cm 高15cm)">
                <span class="dropzone-tip" id="receipt-tip">📷 點擊上傳「廠商施工服務單 / 維修簽認單」<br>(寬 18cm × 高 15cm)</span>
                <img id="receipt-img" alt="廠商服務單">
            </div>
        </div>
    </div>

    <!-- ==================== 第二頁 (對照照片與備註) ==================== -->
    <div class="page-sheet page-2">
        <!-- 第二頁同步頁首物件資訊表（無框線） -->
        <table class="header-table">
            <colgroup>
                <col style="width: 15%;">
                <col style="width: 29%;">
                <col style="width: 15%;">
                <col style="width: 41%;">
            </colgroup>
            <tr>
                <td style="text-align: center;">物件編號</td>
                <td><input type="text" class="sync-prop-id" placeholder="請輸入物件編號" oninput="syncFields('prop-id', this.value)"></td>
                <td style="text-align: right;">房東姓名</td>
                <td><input type="text" class="sync-landlord" value="吳秀珍" oninput="syncFields('landlord', this.value)"></td>
            </tr>
            <tr>
                <td style="text-align: center;">媒合編號</td>
                <td><input type="text" class="sync-match-id" placeholder="請輸入媒合編號" oninput="syncFields('match-id', this.value)"></td>
                <td style="text-align: right;">物件地址</td>
                <td><input type="text" class="sync-address" value="桃園市龜山區文青路163號4樓之6" oninput="syncFields('address', this.value)"></td>
            </tr>
            <tr>
                <td style="text-align: center;">租賃期間</td>
                <td colspan="3">
                    <input type="text" class="sync-lease" value="115/11/01 ~ 116/10/31" oninput="syncFields('lease', this.value)">
                </td>
            </tr>
        </table>

        <!-- 備註與修繕前／中／後對照表 -->
        <table class="compare-table">
            <!-- 備註區 -->
            <tr>
                <td class="col-label">備註</td>
                <td class="col-content">
                    <div class="remarks-container">
                        <div class="remarks-select-row">
                            <select class="remarks-select" id="remarks-select" onchange="applyRemarkTemplate(this.value)">
                                <option value="">⚡ 快速套用修繕標準備註範本（請選擇類別）...</option>

                                <optgroup label="【消防設備】">
                                    <option value="添購滅火器。">添購滅火器</option>
                                    <option value="添購偵煙器。">添購偵煙器</option>
                                    <option value="添購偵煙器及滅火器。">添購偵煙器及滅火器</option>
                                </optgroup>

                                <optgroup label="【冷氣空調】">
                                    <option value="冷氣無法啟動，經師傅評估為內部線路燒掉無法修復，故換新冷氣。">冷氣 - 線路燒毀換新[cite: 2]</option>
                                    <option value="窗型冷氣無法啟動，經師傅評估為內部線路燒掉無法修復，故換新分離式冷氣。">窗型冷氣 - 線路燒毀換新分離式[cite: 2]</option>
                                    <option value="冷氣無法使用，經師傅評估為內部髒污堆積導致無法送風及滴水，故請師傅進行修繕工程。">冷氣 - 髒污滴水修繕[cite: 2]</option>
                                    <option value="冷氣無法製冷，經師傅評估冷媒不足，故進行修繕保養工程。">冷氣 - 冷媒不足保養工程[cite: 2]</option>
                                    <option value="冷氣漏水，經師傅評估為排水器故障無法修復，故換新冷氣排水器。">冷氣 - 排水器故障換新[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【衛浴及給排水設備】">
                                    <option value="水龍頭漏水，經師傅評估無法修復，故換新水龍頭。">水龍頭 - 漏水換新[cite: 2]</option>
                                    <option value="衛浴面盆因裂損導致無法使用，經師傅評估無法修復，故換新面盆。">面盆 - 裂損無法修復換新[cite: 2]</option>
                                    <option value="沐浴龍頭鏽蝕損壞，經師傅評估無法修復，故換新沐浴龍頭。">沐浴龍頭 - 鏽蝕損壞換新[cite: 2]</option>
                                    <option value="排水管漏水，經師傅評估無法修復，故換新排水軟管。">排水軟管 - 漏水無法修復換新[cite: 2]</option>
                                    <option value="排水管線堵塞，故請師傅進行疏通工程。">排水管線 - 堵塞疏通工程[cite: 2]</option>
                                    <option value="馬桶漏水，經師傅評估無法修復，故換新馬桶。">馬桶 - 漏水無法修復換新[cite: 2]</option>
                                    <option value="馬桶水箱漏水，經師傅評估無法修復故換新馬桶水箱。">馬桶水箱 - 漏水無法修復換新[cite: 2]</option>
                                    <option value="馬桶堵塞無法使用，故請師傅進行馬桶疏通工程。">馬桶 - 堵塞疏通工程[cite: 2]</option>
                                    <option value="馬桶漏水，且浴室漏水故請師傅進行全部浴室維修工程。">浴室/馬桶 - 漏水全面維修工程[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【廚房及熱水設備】">
                                    <option value="抽油煙機輪軸斷裂，經師傅評估無法修復，故換新抽油煙機。">抽油煙機 - 輪軸斷裂換新[cite: 2]</option>
                                    <option value="瓦斯爐無法點著，經師傅評估為內部鏽蝕導致無法修復，故換新瓦斯爐。">瓦斯爐 - 鏽蝕無法點著換新[cite: 2]</option>
                                    <option value="熱水器無法點著，經師傅評估為內部鏽蝕導致無法修復，故換新熱水器。">熱水器 - 內部鏽蝕換新[cite: 2]</option>
                                    <option value="熱水器無法點著，經師傅評估為內部鏽蝕，故請師傅進行維修工程。">熱水器 - 內部鏽蝕維修工程[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【居家常用家電】">
                                    <option value="洗衣機轉軸斷裂，經師傅評估無法修復故換新洗衣機。">洗衣機 - 轉軸斷裂換新[cite: 2]</option>
                                    <option value="洗衣機無法運轉，經師傅評估為內部髒污堆積，故請師傅進行修繕工程。">洗衣機 - 髒污堆積修繕工程[cite: 2]</option>
                                    <option value="冰箱壓縮機故障，經師傅評估無法修復故換新冰箱。">冰箱 - 壓縮機故障換新[cite: 2]</option>
                                    <option value="冰箱無法啟動，經師傅評估為電腦基板故障，故進行修復工程。">冰箱 - 電腦基板故障修復[cite: 2]</option>
                                    <option value="電視因顯示面板故障，經師傅評估無法修復故換新電視。">電視 - 面板故障換新[cite: 2]</option>
                                    <option value="除濕機無法啟動，經師傅評估內部電路燒毀無法修復，故換新除濕機。">除濕機 - 電路燒毀換新[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【抽水馬達與加壓泵】">
                                    <option value="馬達無法抽水，經師傅評估無法修復，故換新馬達。">抽水馬達 - 無法抽水換新[cite: 2]</option>
                                    <option value="租屋處無法用水，經師傅評估為加壓馬達內部開關故障，故請師傅進行換修工程。">加壓馬達 - 開關故障換修工程[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【門扇、門鎖與弱電】">
                                    <option value="木門因受潮導致變形無法正常閉合，經師傅評估無法修復故換新門。">木門 - 受潮變形換新門[cite: 2]</option>
                                    <option value="門因氧化脆裂導致無法關門，經師傅評估無法修復故換新門。">門扇 - 氧化脆裂換新門[cite: 2]</option>
                                    <option value="門鎖因鏽蝕導致無法開關，經師傅評估無法修復故換新門鎖。">一般門鎖 - 鏽蝕無法開關換新[cite: 2]</option>
                                    <option value="電子門鎖因電池鏽蝕及內部液體漏出導致無法開關，故進行換修工程。">電子門鎖 - 電池漏液換修工程[cite: 2]</option>
                                    <option value="對講機損壞無法使用，經師傅評估無法修復，故請師傅安裝一對一對講機。">對講機 - 損壞換裝一對一對講機[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【壁癌防水與泥作工程】">
                                    <option value="漏水導致壁癌，故請師傅進行防水油漆粉刷工程。">防水油漆 - 漏水壁癌粉刷工程[cite: 2]</option>
                                    <option value="壁癌導致油漆剝落，故請師傅進行重新粉刷工程。">油漆粉刷 - 壁癌油漆剝落粉刷[cite: 2]</option>
                                    <option value="屋頂漏水至租屋處，故請師傅進行屋頂防水工程。">屋頂防水 - 漏水至屋內防水工程[cite: 2]</option>
                                    <option value="地板磁磚因地震導致變形破裂，經師傅評估無法修復故請師傅進行維修工程。">地板磁磚 - 地震變形破裂維修[cite: 2]</option>
                                </optgroup>

                                <optgroup label="【傢俱與照明設備】">
                                    <option value="因床墊彈簧彈出無法使用，經師傅評估無法修復故換新床墊。">床墊 - 彈簧彈出換新[cite: 2]</option>
                                    <option value="因沙發彈簧彈出無法使用，經師傅評估無法修復故換新沙發。">沙發 - 彈簧彈出換新[cite: 2]</option>
                                    <option value="照明設備無法使用，經師傅評估無法修復故進行維修換新工程。">照明設備 - 無法使用維修換新[cite: 2]</option>
                                </optgroup>
                            </select>
                            <button type="button" class="btn-clear-note" onclick="clearRemarkText()">清空</button>
                        </div>
                        <textarea class="remarks-input" id="remarks-text" placeholder="請填寫修繕品項或說明備註（可由選單帶入並自由編輯修改）">添購滅火器。</textarea>
                    </div>
                </td>
            </tr>

            <!-- 1. 修繕前 -->
            <tr>
                <td class="col-label">修繕前</td>
                <td class="col-content">
                    <div class="multi-photo-wrapper">
                        <input type="file" id="before-file" class="hidden-file-input" accept="image/*" multiple capture="environment" onchange="handleP2PhotoUpload(this, 'before-grid', 'before-btn')">
                        <button type="button" class="btn-add-photos" id="before-btn" onclick="document.getElementById('before-file').click()">
                            📷 新增「修繕前」照片 
                        </button>
                        <div class="photo-gallery-grid" id="before-grid">
                            <div class="empty-photo-tip">尚未上傳修繕前照片</div>
                        </div>
                    </div>
                </td>
            </tr>

            <!-- 2. 修繕中  -->
            <tr>
                <td class="col-label">修繕中</td>
                <td class="col-content">
                    <div class="multi-photo-wrapper">
                        <input type="file" id="during-file" class="hidden-file-input" accept="image/*" multiple capture="environment" onchange="handleP2PhotoUpload(this, 'during-grid', 'during-btn')">
                        <button type="button" class="btn-add-photos" id="during-btn" onclick="document.getElementById('during-file').click()">
                            📷 新增「修繕中」施工照片 
                        </button>
                        <div class="photo-gallery-grid" id="during-grid">
                            <div class="empty-photo-tip">尚未上傳修繕中照片</div>
                        </div>
                    </div>
                </td>
            </tr>

            <!-- 3. 修繕後 (限制最多2張，寬8cm 高8.5cm，滿版無黑邊) -->
            <tr>
                <td class="col-label">修繕後</td>
                <td class="col-content">
                    <div class="multi-photo-wrapper">
                        <input type="file" id="after-file" class="hidden-file-input" accept="image/*" multiple capture="environment" onchange="handleP2PhotoUpload(this, 'after-grid', 'after-btn')">
                        <button type="button" class="btn-add-photos" id="after-btn" onclick="document.getElementById('after-file').click()">
                            📷 新增「修繕後」完工照片 
                        </button>
                        <div class="photo-gallery-grid" id="after-grid">
                            <div class="empty-photo-tip">尚未上傳修繕後照片</div>
                        </div>
                    </div>
                </td>
            </tr>
        </table>
    </div>
</div>

<script>
    // 雙頁欄位雙向自動同步
    function syncFields(fieldClass, value) {
        document.querySelectorAll(`.sync-${fieldClass}`).forEach(el => {
            if (el.value !== value) {
                el.value = value;
            }
        });
    }

    // 備註範本套用
    function applyRemarkTemplate(text) {
        if (!text) return;
        const textarea = document.getElementById('remarks-text');
        textarea.value = text;
        textarea.focus();
    }

    function clearRemarkText() {
        document.getElementById('remarks-text').value = '';
        document.getElementById('remarks-select').value = '';
        document.getElementById('remarks-text').focus();
    }

    // 第一頁：單張圖片預覽處理 
    function previewP1Image(input, imgId, tipId) {
        if (input.files && input.files[0]) {
            const reader = new FileReader();
            reader.onload = function(e) {
                const img = document.getElementById(imgId);
                const tip = document.getElementById(tipId);
                img.src = e.target.result;
                img.style.display = 'block';
                if (tip) tip.style.display = 'none';
            };
            reader.readAsDataURL(input.files[0]);
        }
    }

    // 第二頁：多圖上傳處理
    function handleP2PhotoUpload(input, gridId, btnId) {
        if (!input.files || input.files.length === 0) return;
        const grid = document.getElementById(gridId);
        const btn = document.getElementById(btnId);

        let currentCards = grid.querySelectorAll('.photo-thumb-card').length;
        if (currentCards >= 2) {
            alert('此欄位最多只能放置 2 張照片！');
            input.value = '';
            return;
        }

        // 清除尚未上傳提示文字
        const tip = grid.querySelector('.empty-photo-tip');
        if (tip) tip.remove();

        const filesToProcess = Array.from(input.files).slice(0, 2 - currentCards);

        filesToProcess.forEach(file => {
            const reader = new FileReader();
            reader.onload = function(e) {
                const card = document.createElement('div');
                card.className = 'photo-thumb-card';
                card.innerHTML = `
                    <button type="button" class="photo-thumb-del" onclick="removeP2PhotoCard(this, '${gridId}', '${btnId}')" title="刪除照片">✕</button>
                    <img src="${e.target.result}" alt="照片">
                `;
                grid.appendChild(card);
                checkP2Limit(gridId, btnId);
            };
            reader.readAsDataURL(file);
        });

        input.value = '';
    }

    // 刪除照片卡片
    function removeP2PhotoCard(delBtn, gridId, btnId) {
        const grid = document.getElementById(gridId);
        delBtn.closest('.photo-thumb-card').remove();
        checkP2Limit(gridId, btnId);
        if (grid.querySelectorAll('.photo-thumb-card').length === 0) {
            grid.innerHTML = '<div class="empty-photo-tip">尚未上傳照片</div>';
        }
    }

    // 檢查張數是否滿 2 張，滿了自動隱藏新增按鈕
    function checkP2Limit(gridId, btnId) {
        const grid = document.getElementById(gridId);
        const btn = document.getElementById(btnId);
        const count = grid.querySelectorAll('.photo-thumb-card').length;
        if (count >= 2) {
            btn.style.display = 'none';
        } else {
            btn.style.display = 'inline-block';
        }
    }

    // 匯出 PDF 功能（雙頁完整對齊）
    function exportToPDF() {
        const element = document.getElementById('pdf-export-root');
        
        const address = document.querySelector('.sync-address').value.trim() || '未填地址';
        const landlord = document.querySelector('.sync-landlord').value.trim() || '房東';
        const pdfFileName = `${address}_${landlord}_修繕送件表.pdf`;

        element.classList.add('rendering-pdf');

        const opt = {
            margin:       [0, 0, 0, 0],
            filename:     pdfFileName,
            image:        { type: 'jpeg', quality: 0.98 },
            html2canvas:  { scale: 2, useCORS: true, logging: false },
            pagebreak:    { mode: ['css', 'legacy'] },
            jsPDF:        { unit: 'mm', format: 'a4', orientation: 'portrait' }
        };

        html2pdf().set(opt).from(element).save().then(() => {
            element.classList.remove('rendering-pdf');
        }).catch(err => {
            element.classList.remove('rendering-pdf');
            window.print();
        });
    }
</script>

</body>
</html>

<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قالب الدعم والاقتراحات</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 600px;
            margin: auto;
        }
        .box {
            background-color: #fff;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 15px;
            padding: 15px;
            cursor: pointer;
            transition: 0.3s;
        }
        .box:hover {
            background-color: #e7e7e7;
        }
        .content {
            display: none;
            padding-top: 10px;
        }
        .code-area {
            background-color: #eef;
            border: 1px solid #ccc;
            border-radius: 5px;
            padding: 10px;
            margin-top: 20px;
            white-space: pre-wrap; /* للحفاظ على تنسيق الكود */
            font-family: monospace;
        }
    </style>
</head>
<body>

<div class="container">
    <div class="box" onclick="toggleContent(this)">
        <h3>طلب الدعم</h3>
        <div class="content"><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نموذج طلب دعم</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #e9ecef;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            direction: rtl;
        }

        .container {
            max-width: 90%; /* تعديل لزيادة التناسب مع الهاتف */
            padding: 20px; /* تقليل padding لتناسب الهاتف */
            background: #fff;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            border: 1px solid #ddd;
            text-align: right;
        }

        .logo {
            display: block;
            margin: 0 auto 20px; /* توسيط الشعار مع هوامش مناسبة */
            width: 100px; /* تعديل حجم الشعار */
        }

        h1 {
            color: #004085;
            margin-bottom: 20px;
            font-size: 24px; /* تقليل حجم الخط */
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #333;
        }

        input, select, textarea, button {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 20px;
            font-size: 14px;
            box-sizing: border-box;
            transition: border-color 0.3s ease;
            text-align: right;
        }

        input:focus, select:focus, textarea:focus {
            border-color: #007bff;
            outline: none;
        }

        button {
            background-color: #004085;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #003366;
        }

        #statusMessage {
            text-align: center;
            margin-top: 15px;
            font-size: 16px;
            color: #28a745;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png" alt="شعار" class="logo">
        <h1>نموذج طلب دعم</h1>
        <form id="supportForm">
            <label for="organization">اسم الجهة الحكومية:</label>
            <select id="organization" name="organization" required>
                <option value="وزارة الطاقة والثروة المعدنية" data-whatsapp="+962775573157" data-email="">وزارة الطاقة والثروة المعدنية</option>
                <option value="هيئة تنظيم قطاع الطاقة والمعادن" data-whatsapp="" data-email="info@emrc.gov.jo">هيئة تنظيم قطاع الطاقة والمعادن (EMRC)</option>
                <option value="شركة الكهرباء الوطنية" data-whatsapp="" data-email="info@nepco.com.jo">شركة الكهرباء الوطنية (NEPCO)</option>
                <option value="صندوق تشجيع الطاقة المتجددة وترشيد الطاقة" data-whatsapp="" data-email="info@jreeef.gov.jo">صندوق تشجيع الطاقة المتجددة وترشيد الطاقة (JREEEF)</option>
            </select>
            
            <label for="name">اسمك الكامل:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="nationalID">الرقم الوطني:</label>
            <input type="text" id="nationalID" name="nationalID" required>
            
            <label for="phone">رقم الهاتف:</label>
            <input type="tel" id="phone" name="phone" required>
            
            <label for="email">البريد الإلكتروني:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="issue">المشكلة التي تحتاج الدعم من أجلها:</label>
            <textarea id="issue" name="issue" rows="4" required></textarea>
            
            <button type="button" onclick="openWhatsAppOrEmail()">إرسال</button>
        </form>
        <div id="statusMessage">تم إرسال الطلب بنجاح!</div>
    </div>

    <script>
        function openWhatsAppOrEmail() {
            const name = document.getElementById('name').value;
            const nationalID = document.getElementById('nationalID').value;
            const phone = document.getElementById('phone').value;
            const email = document.getElementById('email').value;
            const issue = document.getElementById('issue').value;
            const organizationElement = document.getElementById('organization');
            const organization = organizationElement.value;
            const whatsappNumber = organizationElement.options[organizationElement.selectedIndex].dataset.whatsapp;
            const emailRecipient = organizationElement.options[organizationElement.selectedIndex].dataset.email;

            if (!name || !nationalID || !phone || !email || !issue) {
                alert("يرجى ملء جميع الحقول.");
                return;
            }

            const message = `
                السادة/ ${organization} المحترمين،

                تحية طيبة وبعد،

                أود أن أرفع إلى مقامكم طلب الدعم حول الموضوع التالي:

                المشكلة: ${issue}.

                أود من حضرتكم النظر في طلبي والتكرم باتخاذ اللازم لإيجاد حل لهذه المشكلة.

                بياناتي هي كالتالي:
                - الاسم الكامل: ${name}
                - الرقم الوطني: ${nationalID}
                - رقم الهاتف: ${phone}
                - البريد الإلكتروني: ${email}

                أرجو منكم التواصل معي في أقرب وقت ممكن لمتابعة هذا الطلب.

                وتفضلوا بقبول فائق الاحترام والتقدير.

                ${name}
            `;

            if (whatsappNumber) {
                const whatsappURL = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
                window.open(whatsappURL, '_blank');
            } else if (emailRecipient) {
                const subject = `طلب دعم من ${name}`;
                const emailURL = `mailto:${emailRecipient}?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(message)}`;
                window.location.href = emailURL;
            }

            document.getElementById('statusMessage').style.display = 'block';
            document.getElementById('supportForm').reset();
        }
    </script>
</body>
</html>
</div>
    </div>

    <div class="box" onclick="toggleContent(this)">
        <h3>اقتراحات نشمية</h3>
        <div class="content"><!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نموذج تقديم اقتراح</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #e9ecef;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            direction: rtl;
        }

        .container {
            max-width: 90%; /* جعل العرض أقصى 90% ليتناسب مع الهاتف */
            padding: 20px; /* تقليل padding لتناسب الهاتف */
            background: #fff;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            border: 1px solid #ddd;
            text-align: right;
        }

        .logo {
            display: block;
            margin: 0 auto 20px; /* توسيط الشعار */
            width: 100px; /* حجم الشعار */
        }

        h1 {
            color: #004085;
            margin-bottom: 20px;
            font-size: 24px; /* تقليل حجم الخط */
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #333;
        }

        input, select, textarea, button {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 5px;
            margin-bottom: 20px;
            font-size: 14px;
            box-sizing: border-box;
            transition: border-color 0.3s ease;
            text-align: right;
        }

        input:focus, select:focus, textarea:focus {
            border-color: #007bff;
            outline: none;
        }

        button {
            background-color: #004085;
            color: white;
            border: none;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #003366;
        }

        #statusMessage {
            text-align: center;
            margin-top: 15px;
            font-size: 16px;
            color: #28a745;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png" alt="شعار" class="logo"> <!-- الشعار المطلوب -->
        <h1>نموذج تقديم اقتراح</h1>
        <form id="suggestionForm">
            <label for="organization">اسم الجهة الحكومية:</label>
            <select id="organization" name="organization" required>
                <option value="وزارة الطاقة والثروة المعدنية">وزارة الطاقة والثروة المعدنية</option>
                <option value="هيئة تنظيم قطاع الطاقة والمعادن (EMRC)">هيئة تنظيم قطاع الطاقة والمعادن (EMRC)</option>
                <option value="شركة الكهرباء الوطنية (NEPCO)">شركة الكهرباء الوطنية (NEPCO)</option>
                <option value="صندوق تشجيع الطاقة المتجددة وترشيد الطاقة (JREEEF)">صندوق تشجيع الطاقة المتجددة وترشيد الطاقة (JREEEF)</option>
            </select>
            
            <label for="name">اسمك الكامل:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="nationalID">الرقم الوطني:</label>
            <input type="text" id="nationalID" name="nationalID" required>
            
            <label for="phone">رقم الهاتف:</label>
            <input type="tel" id="phone" name="phone" required>
            
            <label for="email">البريد الإلكتروني:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="suggestion">تفاصيل الاقتراح:</label>
            <textarea id="suggestion" name="suggestion" rows="4" required></textarea>
            
            <button type="button" onclick="sendToWhatsApp()">إرسال</button>
        </form>
        <div id="statusMessage">تم إرسال الاقتراح بنجاح!</div>
    </div>

    <script>
        function sendToWhatsApp() {
            const name = document.getElementById('name').value;
            const nationalID = document.getElementById('nationalID').value;
            const phone = document.getElementById('phone').value;
            const email = document.getElementById('email').value;
            const suggestion = document.getElementById('suggestion').value;
            const organization = document.getElementById('organization').value;

            if (!name || !nationalID || !phone || !email || !suggestion) {
                alert("يرجى ملء جميع الحقول.");
                return;
            }

            const message = `
                السادة/ ${organization} المحترمين،

                تحية طيبة وبعد،

                أود أن أرفع إلى مقامكم هذا الاقتراح:

                تفاصيل الاقتراح: ${suggestion}.

                بياناتي هي كالتالي:
                - الاسم الكامل: ${name}
                - الرقم الوطني: ${nationalID}
                - رقم الهاتف: ${phone}
                - البريد الإلكتروني: ${email}

                وتفضلوا بقبول فائق الاحترام والتقدير.

                ${name}
            `;

            const whatsappNumber = '962781339210'; // الرقم الموحد لجميع الرسائل (بدون +)
            const whatsappURL = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
            window.open(whatsappURL, '_blank');

            document.getElementById('statusMessage').style.display = 'block';
            document.getElementById('suggestionForm').reset();
        }
    </script>
</body>
</html>
</div>
    </div>

    <div class="box" onclick="toggleContent(this)">
        <h3>شركات الطاقة الشمسية</h3>
        <div class="content"><!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>صفحة شركات الطاقة الشمسية في الأردن</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .header {
            background-color: #004085;
            color: white;
            width: 100%;
            padding: 20px;
            text-align: center;
        }
        .header img {
            width: 100px;
            margin-bottom: 10px;
        }
        .search-container {
            margin: 20px;
            width: 100%;
            max-width: 600px; /* تحديد عرض أقصى للحقل */
        }
        .search-box {
            width: 100%;
            padding: 10px;
            font-size: 16px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .company-list {
            width: 100%;
            max-width: 600px; /* تحديد عرض أقصى للقائمة */
            margin: 20px auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 15px;
        }
        .company {
            margin: 10px 0;
            border-bottom: 1px solid #eee;
            padding: 10px 0;
        }
        .company:last-child {
            border-bottom: none; /* إزالة الخط الأخير */
        }
        .company-title {
            font-weight: bold;
            color: #004085;
        }
        .company-email {
            color: #007BFF;
            text-decoration: none;
        }
        .company-email:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="header">
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png"شعار الصفحة"> <!-- استبدل الرابط برابط الشعار الخاص بك -->
        <h1>شركات الطاقة الشمسية في الأردن</h1>
    </div>

    <div class="search-container">
        <input type="text" id="searchInput" class="search-box" placeholder="ابحث عن شركة..." onkeyup="searchCompanies()">
    </div>

    <div class="company-list" id="companyList">
        <div class="company">
            <span class="company-title">شركة الفنار للطاقة الشمسية</span><br>
            <a href="mailto:info@alfanar.com" class="company-email">info@alfanar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة نور الأردن للطاقة الشمسية</span><br>
            <a href="mailto:info@noorjo.com" class="company-email">info@noorjo.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إيست كروب للطاقة</span><br>
            <a href="mailto:info@eastgroupenergy.com" class="company-email">info@eastgroupenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة فينيكس للطاقة الشمسية</span><br>
            <a href="mailto:info@phoenixsolarenergy.com" class="company-email">info@phoenixsolarenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة الدار للطاقة</span><br>
            <a href="mailto:info@aldarenergy.com" class="company-email">info@aldarenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة طاقة الرياح والطاقة الشمسية</span><br>
            <a href="mailto:info@wspc.com" class="company-email">info@wspc.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة ميدل إيست للطاقة</span><br>
            <a href="mailto:info@middleeastenergy.com" class="company-email">info@middleeastenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إيفكو للطاقة</span><br>
            <a href="mailto:info@efcoenergy.com" class="company-email">info@efcoenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة كريستال للطاقة</span><br>
            <a href="mailto:info@crystalenergy.com" class="company-email">info@crystalenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة طاقة الأردن</span><br>
            <a href="mailto:info@jordanenergy.com" class="company-email">info@jordanenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار تيك للطاقة الشمسية (SolarTech)</span><br>
            <a href="mailto:info@solartechjo.com" class="company-email">info@solartechjo.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة أونيرا للطاقة الشمسية (Onira Solar)</span><br>
            <a href="mailto:info@onirasolar.com" class="company-email">info@onirasolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سكاي لاين للطاقة الشمسية (Skyline Solar)</span><br>
            <a href="mailto:info@skylinesolar.com" class="company-email">info@skylinesolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة أبتيموس للطاقة الشمسية (Optimus Energy)</span><br>
            <a href="mailto:info@optimusenergy.com" class="company-email">info@optimusenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة فيوتشر للطاقة الشمسية (Future Solar)</span><br>
            <a href="mailto:info@futuresolar.com" class="company-email">info@futuresolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة بتر سولار (Better Solar)</span><br>
            <a href="mailto:info@bettersolar.com" class="company-email">info@bettersolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة بوش للطاقة الشمسية (Bosch Solar)</span><br>
            <a href="mailto:info@boschsolar.com" class="company-email">info@boschsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة النسر للطاقة الشمسية (Eagle Solar)</span><br>
            <a href="mailto:info@eaglesolar.com" class="company-email">info@eaglesolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سيبكو للطاقة الشمسية (SEPCO Solar)</span><br>
            <a href="mailto:info@sepcosolar.com" class="company-email">info@sepcosolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة جرين ويف للطاقة الشمسية (Green Wave Energy)</span><br>
            <a href="mailto:info@greenwaveenergy.com" class="company-email">info@greenwaveenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة المستقبل للطاقة الشمسية (Future Energy Solar)</span><br>
            <a href="mailto:info@futureenergysolar.com" class="company-email">info@futureenergysolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة أومني للطاقة الشمسية (Omni Energy)</span><br>
            <a href="mailto:info@omnienergy.com" class="company-email">info@omnienergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة بيكاسوس للطاقة الشمسية (Pegasus Solar)</span><br>
            <a href="mailto:info@pegasussolar.com" class="company-email">info@pegasussolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سكاي إنرجي للطاقة الشمسية (Sky Energy)</span><br>
            <a href="mailto:info@skyenergy.com" class="company-email">info@skyenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة نيوم للطاقة الشمسية (Neom Solar)</span><br>
            <a href="mailto:info@neomsolar.com" class="company-email">info@neomsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إل جي للطاقة الشمسية (LG Solar)</span><br>
            <a href="mailto:info@lgsolar.com" class="company-email">info@lgsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة أكسيس للطاقة الشمسية (Axis Energy)</span><br>
            <a href="mailto:info@axisenergy.com" class="company-email">info@axisenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة ألفا للطاقة الشمسية (Alpha Solar)</span><br>
            <a href="mailto:info@alphasolar.com" class="company-email">info@alphasolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إنيرجي تيك للطاقة الشمسية (EnergyTech Solar)</span><br>
            <a href="mailto:info@energytechsolar.com" class="company-email">info@energytechsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة تروبيكال للطاقة الشمسية (Tropical Solar)</span><br>
            <a href="mailto:info@tropicalsolar.com" class="company-email">info@tropicalsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة صن باور للطاقة الشمسية (SunPower Solar)</span><br>
            <a href="mailto:info@sunpower.com" class="company-email">info@sunpower.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة مايكرو سولار للطاقة الشمسية (MicroSolar Energy)</span><br>
            <a href="mailto:info@microsolar.com" class="company-email">info@microsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار بلس للطاقة الشمسية (SolarPlus Energy)</span><br>
            <a href="mailto:info@solarplus.com" class="company-email">info@solarplus.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة كلير إنرجي للطاقة الشمسية (Clear Energy)</span><br>
            <a href="mailto:info@clearenergy.com" class="company-email">info@clearenergy.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة جولدن صن للطاقة الشمسية (Golden Sun Solar)</span><br>
            <a href="mailto:info@goldensun.com" class="company-email">info@goldensun.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سيستم سولار للطاقة الشمسية (System Solar)</span><br>
            <a href="mailto:info@systemsolar.com" class="company-email">info@systemsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة باور سولار للطاقة الشمسية (Power Solar)</span><br>
            <a href="mailto:info@powersolar.com" class="company-email">info@powersolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار ترست للطاقة الشمسية (SolarTrust)</span><br>
            <a href="mailto:info@solartrust.com" class="company-email">info@solartrust.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إيليت سولار للطاقة الشمسية (Elite Solar)</span><br>
            <a href="mailto:info@elitesolar.com" class="company-email">info@elitesolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة أدفانسد للطاقة الشمسية (Advanced Solar)</span><br>
            <a href="mailto:info@advancedsolar.com" class="company-email">info@advancedsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إيكو سولار للطاقة الشمسية (EcoSolar)</span><br>
            <a href="mailto:info@ecosolar.com" class="company-email">info@ecosolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار إنرجي سولوشنز (Solar Energy Solutions)</span><br>
            <a href="mailto:info@solarenergysolutions.com" class="company-email">info@solarenergysolutions.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار تكنولوجيز (Solar Technologies)</span><br>
            <a href="mailto:info@solartechnologies.com" class="company-email">info@solartechnologies.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إنيرجي كير للطاقة الشمسية (EnergyCare Solar)</span><br>
            <a href="mailto:info@energycaresolar.com" class="company-email">info@energycaresolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة ترو سكيب للطاقة الشمسية (TrueScape Solar)</span><br>
            <a href="mailto:info@truescapesolar.com" class="company-email">info@truescapesolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إنفينيتي للطاقة الشمسية (Infinity Solar)</span><br>
            <a href="mailto:info@infinitysolar.com" class="company-email">info@infinitysolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة بلو سكاي للطاقة الشمسية (Blue Sky Solar)</span><br>
            <a href="mailto:info@blueskysolar.com" class="company-email">info@blueskysolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولايت للطاقة الشمسية (Solight Solar)</span><br>
            <a href="mailto:info@solightsolar.com" class="company-email">info@solightsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة جي إس للطاقة الشمسية (GS Solar)</span><br>
            <a href="mailto:info@gssolar.com" class="company-email">info@gssolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة تيتان للطاقة الشمسية (Titan Solar)</span><br>
            <a href="mailto:info@titansolar.com" class="company-email">info@titansolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إنيرجي برو للطاقة الشمسية (EnergyPro Solar)</span><br>
            <a href="mailto:info@energyprosolar.com" class="company-email">info@energyprosolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة بريمير للطاقة الشمسية (Premier Solar)</span><br>
            <a href="mailto:info@premiersolar.com" class="company-email">info@premiersolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة فيجن للطاقة الشمسية (Vision Solar)</span><br>
            <a href="mailto:info@visionsolar.com" class="company-email">info@visionsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار تك للطاقة الشمسية (Solar Tech)</span><br>
            <a href="mailto:info@solartech.com" class="company-email">info@solartech.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إنيشيال للطاقة الشمسية (Initial Solar)</span><br>
            <a href="mailto:info@initialsolar.com" class="company-email">info@initialsolar.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة سولار إنرجايزر (Solar Energizer)</span><br>
            <a href="mailto:info@solarenergizer.com" class="company-email">info@solarenergizer.com</a>
        </div>
        <div class="company">
            <span class="company-title">شركة إيليت للطاقة الشمسية (Elite Energy)</span><br>
            <a href="mailto:info@eliteenergy.com" class="company-email">info@eliteenergy.com</a>
        </div>
    </div>

    <script>
        function searchCompanies() {
            const input = document.getElementById('searchInput');
            const filter = input.value.toLowerCase();
            const companyList = document.getElementById('companyList');
            const companies = companyList.getElementsByClassName('company');

            for (let i = 0; i < companies.length; i++) {
                const title = companies[i].getElementsByClassName('company-title')[0];
                if (title) {
                    const txtValue = title.textContent || title.innerText;
                    companies[i].style.display = txtValue.toLowerCase().includes(filter) ? '' : 'none';
                }
            }
        }
    </script>
</body>
</html>
</div>
    </div>

    <div class="box" onclick="toggleContent(this)">
        <h3>مشاريع القائمة في المملكة الأردنية الهاشمية</h3>
        <div class="content"><!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قائمة مشاريع الطاقة المتجددة في الأردن</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #e9ecef; /* لون خلفية أكثر رسمية */
        }
        header {
            background-color: #004b87; /* لون رمزي للحكومة */
            color: white;
            padding: 20px;
            text-align: center;
        }
        header img {
            width: 100px; /* عرض الشعار */
            margin-bottom: 10px;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }
        .container {
            max-width: 900px;
            margin: 20px auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            box-sizing: border-box;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #007bff; /* لون مميز للعناوين */
            color: white;
        }
        td {
            background-color: #ffffff;
        }
        label, select {
            display: block;
            margin: 10px 0;
            width: 100%;
            box-sizing: border-box;
        }
        button {
            background-color: #28a745; /* لون الزر */
            color: white;
            padding: 10px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: #218838; /* لون الزر عند التمرير */
        }
        @media (max-width: 600px) {
            h1 {
                font-size: 20px; /* حجم خط أصغر على الهواتف */
            }
            th, td {
                padding: 8px;
                font-size: 14px; /* حجم خط أصغر على الهواتف */
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png" alt="شعار الأردن">
        <h1>قائمة مشاريع الطاقة المتجددة في الأردن</h1>
    </header>
    
    <div class="container">
        <label for="locationFilter">اختر الموقع:</label>
        <select id="locationFilter" onchange="filterProjects()">
            <option value="">اختر المحافظة</option>
            <option value="Tafileh">الطفيلة</option>
            <option value="Mafraq">المفرق</option>
            <option value="Maan">معان</option>
            <option value="Aqaba">العقبة</option>
            <option value="Zarqaa">الزرقاء</option>
            <option value="Amman">عمان</option>
        </select>

        <table id="projectsTable">
            <thead>
                <tr>
                    <th>اسم المشروع</th>
                    <th>حالة المشروع</th>
                    <th>الموقع</th>
                    <th>اسم المالك</th>
                    <th>حجم المشروع (MWAC)</th>
                    <th>جهة الاتصال</th>
                </tr>
            </thead>
            <tbody>
                <!-- Tafileh Projects -->
                <tr data-location="Tafileh">
                    <td>Jordan Wind Farm</td>
                    <td>Operational since September 2015</td>
                    <td>الطفيلة</td>
                    <td>JWPC</td>
                    <td>117</td>
                    <td><a href="mailto: mjallad@jordanwind.com">mjallad@jordanwind.com</a></td>
                </tr>
                <tr data-location="Tafileh">
                    <td>Wind energy project - Mass</td>
                    <td>Operational since July 2020</td>
                    <td>الطفيلة</td>
                    <td>Mass Energy</td>
                    <td>100</td>
                    <td><a href="mailto: khaled.abualshaikh@massgroupholding.com">khaled.abualshaikh@massgroupholding.com</a></td>
                </tr>
                <!-- Mafraq Projects -->
                <tr data-location="Mafraq">
                    <td>Al-Badiya Philadelphia</td>
                    <td>Operational since October 2015</td>
                    <td>المفرق</td>
                    <td>Philadelphia Solar</td>
                    <td>13</td>
                    <td><a href="mailto: a.smadi@philadelphia-solar.com">a.smadi@philadelphia-solar.com</a></td>
                </tr>
                <tr data-location="Mafraq">
                    <td>Direct Proposal/ Round 1 PV/ Jordan Solar One</td>
                    <td>Operational since September 2016</td>
                    <td>المفرق</td>
                    <td>Jordan Solar One</td>
                    <td>20</td>
                    <td><a href="mailto: Projects.jordan@outlook.com">Projects.jordan@outlook.com</a></td>
                </tr>
                <!-- Maan Projects -->
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ Scatec Solar</td>
                    <td>Operational since June 2016</td>
                    <td>معان</td>
                    <td>Scatec Solar</td>
                    <td>10</td>
                    <td><a href="mailto: iyad.assaf@scatecsolar.com">iyad.assaf@scatecsolar.com</a></td>
                </tr>
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ SunEdison Project</td>
                    <td>Operational since July 2016</td>
                    <td>معان</td>
                    <td>Adwa’a Maân</td>
                    <td>20</td>
                    <td><a href="mailto: mahmoud_alhamaideh@ctgsail.com">mahmoud_alhamaideh@ctgsail.com</a></td>
                </tr>
                <!-- Aqaba Projects -->
                <tr data-location="Aqaba">
                    <td>Direct proposals/ Round 1 PV/ Shamsuna</td>
                    <td>Operational since February 2016</td>
                    <td>العقبة</td>
                    <td>Shamsuna</td>
                    <td>10</td>
                    <td><a href="mailto: Tamerk@falconmaan.com">Tamerk@falconmaan.com</a></td>
                </tr>
                <tr data-location="Aqaba">
                    <td>Al-Qweira PV Plant - Gulf Grant</td>
                    <td>Operational since July 2018</td>
                    <td>العقبة</td>
                    <td>Government</td>
                    <td>92</td>
                    <td><a href="mailto: okasasbeh@sepco.com.jo">okasasbeh@sepco.com.jo</a></td>
                </tr>
                <!-- Zarqaa Projects -->
                <tr data-location="Zarqaa">
                    <td>Azraq Camp Solar PV Plant</td>
                    <td>Operational since April 2015</td>
                    <td>الزرقاء</td>
                    <td>Government</td>
                    <td>2</td>
                    <td><a href="mailto: smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <tr data-location="Zarqaa">
                    <td>Expansion of Azraq PV plant</td>
                    <td>Operational since February 2020</td>
                    <td>الزرقاء</td>
                    <td>Government</td>
                    <td>5</td>
                    <td><a href="mailto: smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <!-- Amman Projects -->
                <tr data-location="Amman">
                    <td>East Amman PV project</td>
                    <td>Operational since September 2019</td>
                    <td>عمان</td>
                    <td>AES/Mitsui</td>
                    <td>40</td>
                    <td><a href="mailto: khaled.othman@aes.com">khaled.othman@aes.com</a></td>
                </tr>
                <tr data-location="Amman">
                    <td>Baynona PV project</td>
                    <td>Operational since December 2020</td>
                    <td>عمان</td>
                    <td>Masdar</td>
                    <td>200</td>
                    <td><a href="mailto: malmasri@baynouna.jo">malmasri@baynouna.jo</a></td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
        function filterProjects() {
            const locationFilter = document.getElementById('locationFilter').value;
            const tableRows = document.querySelectorAll('#projectsTable tbody tr');
            const projectsTable = document.getElementById('projectsTable');

            if (locationFilter) {
                projectsTable.style.display = 'table'; // Show the table
                tableRows.forEach(row => {
                    const location = row.getAttribute('data-location');
                    row.style.display = location === locationFilter ? '' : 'none';
                });
            } else {
                projectsTable.style.display = 'none'; // Hide the table if no location is selected
            }
        }
    </script>
</body>
</html>
</div>
    </div>

    <div class="box" onclick="toggleContent(this)">
        <h3>مواقع الطاقة الشمسية الحكومية في الأردن</h3>
        <div class="content"><!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الجهات الحكومية المعنية بالطاقة والكهرباء</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 20px;
            direction: rtl; /* الاتجاه من اليمين إلى اليسار */
        }

        header {
            background-color: #004b87; /* لون خلفية رأس الصفحة */
            color: #ffffff;
            padding: 10px;
            text-align: center;
        }

        h1 {
            margin: 0;
        }

        .container {
            background-color: #ffffff;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            padding: 20px;
            margin-top: 20px;
        }

        ul {
            list-style-type: none; /* إزالة نقاط القائمة */
            padding: 0;
        }

        li {
            margin: 10px 0;
        }

        a {
            text-decoration: none; /* إزالة التسطير من الروابط */
            color: #004b87; /* لون النص */
            transition: color 0.3s; /* تأثير انتقال اللون */
        }

        a:hover {
            color: #007bff; /* لون عند التمرير على الرابط */
        }

        footer {
            text-align: center;
            margin-top: 20px;
            font-size: 0.8em;
            color: #666;
        }
    </style>
</head>
<body>

<header>
    <h1>الجهات الحكومية المعنية بالطاقة والكهرباء</h1>
</header>

<div class="container">
    <ul>
        <li><a href="https://www.memr.gov.jo/" target="_blank">وزارة الطاقة والثروة المعدنية</a></li>
        <li><a href="https://www.emrc.gov.jo/" target="_blank">هيئة تنظيم قطاع الطاقة والمعادن</a></li>
        <li><a href="https://www.nepco.com.jo/" target="_blank">شركة الكهرباء الوطنية (NEPCO)</a></li>
        <li><a href="https://www.jec.com.jo/" target="_blank">مؤسسة الكهرباء الأردنية</a></li>
        <li><a href="https://www.jordanrenewableenergy.com/" target="_blank">الهيئة الأردنية لمصادر الطاقة المتجددة</a></li>
        <li><a href="http://www.moenv.gov.jo/" target="_blank">وزارة البيئة</a></li>
        <li><a href="https://www.jic.gov.jo/" target="_blank">الهيئة العامة للاستثمار</a></li>
        <li><a href="http://www.dos.gov.jo/" target="_blank">مؤسسة الإحصاءات العامة</a></li>
        <li><a href="http://www.mop.gov.jo/" target="_blank">وزارة التخطيط والتعاون الدولي</a></li>
        <li><a href="http://www.jorenergy.com/" target="_blank">الشركة الأردنية لتوليد الكهرباء</a></li>
    </ul>
</div>

<footer>
    © 2024 - جميع الحقوق محفوظة
</footer>

</body>
</html>
</div>
    </div>

    <div class="code-area">
       
<script>
    function toggleContent(element) {
        // إغلاق جميع المحتويات المفتوحة
        const allContents = document.querySelectorAll('.content');
        allContents.forEach(content => {
            content.style.display = 'none';
        });

        // فتح المحتوى الخاص بالخانة المحددة
        const content = element.querySelector('.content');
        content.style.display = 'block';
    }
</script>

</body>
</html>

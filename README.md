<!DOCTYPE html>
<html dir="rtl" lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>إصدار شهادة صحية</title>
    
    
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Cairo', sans-serif;
        }

        body {
            background-color: #f5f5f5;
            direction: rtl;
        }

        /* Splash Screen Styles */
        .splash-screen {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            animation: fadeSplash 2s ease-in-out forwards;
        }

        .splash-screen img {
            width: 350px;
            height: auto;
        }

        @keyframes fadeSplash {
            0% {
                opacity: 1;
                visibility: visible;
            }
            90% {
                opacity: 1;
                visibility: visible;
            }
            100% {
                opacity: 0;
                visibility: hidden;
            
            }
            
    
                
                
     }              

    .header {
            background-color: #006C67;
            padding: 15px 37px;
            display: flex;
            flex-direction: row-reverse;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            top: 0;
            right: 0;
            left: 0;
            z-index: 1000;
        }

        .menu-icon {
            color: white;
            font-size: 24px;
            cursor: pointer;
        }

        .logo img {
            height: 45px;
            width: auto;
        }

        /* Updated Menu Styles */
        .menu-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-color: rgba(0, 0, 0, 0.5);
            display: none;
            z-index: 998;
         }

        .side-menu {
            position: fixed;
            top: -100vh;
            right: 0;
            left: 0;
            background-color: #006C67;
            z-index: 999;
            transition: top 0.3s ease;
            padding:41px 20px 20px;
        }

        .menu-open .side-menu {
            top: 0;
        }

        .menu-open .menu-overlay {
            display: block;
        }

        .menu-items {
            display: flex;
            flex-direction: column;
            padding: 1.5px;
        }

        .menu-item {
            color: white;
            text-decoration: none;
            padding: 8px 0.2px;
            font-size: 15.2px;
            border-bottom: 0px solid rgba(255, 255, 255, 0.1);
            transition: background-color 0.3s ease;
        }

        .menu-item:hover {
            background-color: rgba(255, 255, 255, 0.1);
        }

        .container {
            max-width: 600px;
            margin: 90px auto 0;
            padding: 50px;
            background-color: #fff;
        }

        .title {
            text-align: center;
            margin: 29px 0 30px;
            font-size: 24px;
            color: #4D4D4F;
            font-weight: 700;
        }

        .profile-photo {
            width: 150px;
            height: 200px;
            margin: 20px auto 30px;
            display: block;
            object-fit: cover;
            border: 1px solid #ddd;
        }

        .form-group {
            margin-top: 18px;
            margin-bottom: 12px;
            background-color: #F5F9FC;
            border-radius: 5px;
            padding: 12px 15px;
            border: 1px solid #E5E9EB;
            position: relative;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .section-title {
            color: #000;
            font-size: 14.2px;
            font-weight: bold;
            position: absolute;
            top: -15px;
            right: 0;
            background-color:;
            padding: 0 8px;
        }

        .form-value {
            color: #4D4D4F;
            font-size: 14px;
            word-wrap: break-word;
            line-height: 1.4;
            padding: 4.5px 0;
        }

        .footer {
            text-align: center;
            padding: 20px 20px 20px;
            margin-top: 40px;
            border-top: 25px solid #eee;
        }

        .footer-text {
            color: #666;
            font-size: 10px;
            margin-bottom: 15px;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            color: #666;
            font-size: 10px;
        }

        .footer-links a {
            color: #666;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-links a:hover {
            color: #006C67;
        }

        @media (max-width: 768px) {
            .container {
                padding: 15px;
            }
            .title {
                font-size: 28.5px;
            }
            .form-group {
                padding: 10px 12px;
            }
            .form-value {
                font-size: 13px;
            }
        }
        
        footer img {
            height : 55px;
        }
        
        
        .dropdown {
    position: relative;
    width: 100%;
    direction: rtl;
}

.dropdown-title {
    color: white;
    padding: 15px;
    cursor: pointer;
    font-size: 16px;
    list-style: none;
}

.dropdown-title::-webkit-details-marker {
    display: none;
}

/* السهم بجانب كلمة الخدمات */
.dropdown-title::after {
    content: '▼';
    margin-right: 10px;
    font-size: 12px;
}

/* عند فتح القائمة يتم تدوير السهم */
details[open] .dropdown-title::after {
    content: '▲';
}

.dropdown-content {
    background: white;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.section {
    margin-bottom: 20px;
}

.section h3 {
    color: #333;
    font-size: 16px;
    margin-bottom: 10px;
}

.dropdown-content a {
    display: block;
    color: #4D4D4F;
    text-decoration: none;
    padding: 8px 0;
    font-size: 14px;
}

.services-list {
    background: #006C67;
    color: white !important;
    text-align: center;
    padding: 12px !important;
    border-radius: 4px;
    margin: 15px 0;
}

.new-badge {
    background-color: #B7D5A3;
    color: #fff;
    font-size: 12px;
    padding: 2px 8px;
    border-radius: 4px;
    margin-right: 8px;
    font-weight: 500;
    display: inline-block;
}

/* تأثير التحويم على الروابط */
.dropdown-content a:hover {
    color: #006C67;
}


.dropdown {
    position: relative;
    width: 100%;
    direction: rtl;
}

.dropdown-title {
    color: #B7D5A3; /* اللون الأخضر الفاتح */
    padding: 15px;
    cursor: pointer;
    font-size: 16px;
    list-style: none;
    font-weight: 500;
}

.dropdown-title::-webkit-details-marker {
    display: none;
}

/* السهم بجانب العنوان */
.dropdown-title::after {
    content: '▼';
    margin-right: 10px;
    font-size: 12px;
}

/* تدوير السهم عند فتح القائمة */
details[open] .dropdown-title::after {
    content: '▲';
}

.dropdown-content {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.about-section h2 {
    color: #000;
    font-size: 18px;
    margin-bottom: 20px;
    font-weight: bold;
}

.links-list {
    display: flex;
    flex-direction: column;
    gap: 12px;
}

.menu-link {
    color: #666;
    text-decoration: none;
    font-size: 14px;
    padding: 8px 0;
    transition: color 0.3s ease;
}

.menu-link:hover {
    color: #006C67;
}

/* تنسيق الرابط النشط */
.menu-link.active {
    color: #000;
    font-weight: bold;
}

/* تخصيص الخلفية البيضاء */
.dropdown-content {
    background: #fff;
    max-height: 80vh; /* ارتفاع أقصى للقائمة */
    overflow-y: auto; /* إضافة شريط تمرير عند الحاجة */
}

/* تنسيق شريط التمرير */
.dropdown-content::-webkit-scrollbar {
    width: 5px;
}

.dropdown-content::-webkit-scrollbar-thumb {
    background: #ccc;
    border-radius: 5px;
}


.form-group {
    margin-top: 18px;
    margin-bottom: 12px;
    background-color: #F5F9FC;
    border-radius: 5px;
    padding: 12px 15px;
    border: 1px solid #E5E9EB;
    position: relative;
    transition: all 0.3s ease;
    cursor: pointer;
}

/* إضافة التأثير عند الضغط */
.form-group:active {
    background-color: #ffffff;
    border: 1px solid #006C67;
    box-shadow: 0 0 0 1px #006C67;
}

.form-group:hover {
    border-color: #006C67;
}

.form-group .section-title {
    color: #000;
    font-size: 14.2px;
    font-weight: bold;
    position: absolute;
    top: -15px;
    right: 0;
    background-color: #fff;
    padding: 0 8px;
    z-index: 1;
}

.form-group .form-value {
    color: #4D4D4F;
    font-size: 14px;
    word-wrap: break-word;
    line-height: 1.4;
    padding: 4.5px 0;
}

/* تأثير النص عند الضغط */
.form-group:active .form-value {
    color: #006C67;
}

.dropdown {
    position: relative;
    width: 102%;
    direction: rtl;
}

.dropdown-title {
    color: #fff;
    padding: 14.5px;
    cursor: pointer;
    font-size: 16px;
    list-style: none;
    font-weight: 500;
}

.dropdown-title::-webkit-details-marker {
    display: none;
}

/* السهم بجانب العنوان */
.dropdown-title::after {
    content: '▼';
    margin-right: 0.5px;
    font-size: 15px;
}

/* تدوير السهم عند فتح القائمة */
details[open] .dropdown-title::after {
    content: '▼';
}

.dropdown-content {
    background: white;
    padding: 20px;
    border-radius: 0px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    max-height: 66vh; /* ارتفاع أقصى للقائمة */
    overflow-y: auto; /* إضافة شريط تمرير */
    width: 95%; /* عرض القائمة - يمكنك تعديله حسب الحاجة */
    margin: 10 auto; /* توسيط القائمة */
}

.section-title {
    color: #000;
    font-size: 17px;
    margin: 1px  ;
    font-weight: bold;
}

.links-list {
    display: flex;
    flex-direction: column;
    gap: 12px;
    margin-bottom: 10px;
}

.menu-link {
    color: #666;
    text-decoration: none;
    font-size: 14px;
    padding: 8px 0;
    transition: color 0.3s ease;
    display: block;
}

.menu-link:hover {
    color: #006C67;
}

/* تنسيق شريط التمرير */
.dropdown-content::-webkit-scrollbar {
    width: 5px;
}

.dropdown-content::-webkit-scrollbar-track {
    background: #f1f1f1;
    border-radius: 0px;
}

.dropdown-content::-webkit-scrollbar-thumb {
    background: #888;
    border-radius: 0px;
}

.dropdown-content::-webkit-scrollbar-thumb:hover {
    background: #555;
}

/* تعديل العرض للشاشات المختلفة */
@media (max-width: 700px) {
    .dropdown-content {
        width: 85%;
    }
}


.froom-title {
    color: #fff;
    padding: 15px;
    cursor: pointer;
    font-size: 16px;
    list-style: none;
    font-weight: 500;            
    </style>
</head>
<body>
    <!-- Splash Screen -->
    <div class="splash-screen">
        <img src="https://i.ibb.co/BttsMQB/Screenshot-20241025-132635.jpg" alt="Screenshot-20241025-132635" border="0" /></a>
    </div>





    <header class="header">
              
        <div class="menu-icon">☰</div>
        <div class="logo">
            
            
            
            <img src="https://i.ibb.co/PgQNZqf/1000923069.png" alt="1000923069" border="0" /></a>
        </div>
    </header>

    <!-- Menu Overlay and Side Menu -->
    <div class="menu-overlay"></div>
    <div class="side-menu">
        <div class="menu-items">
            <a href="#" class="menu-item"></a> 
            
            <div class="menu">
    <details class="dropdown">
        <summary class="dropdown-title">عن بلدي</summary>
        <div class="dropdown-content">
            <div class="about-section">
                <h2>من نحن</h2>
                
                <div class="links-list">
                    <a href="#" class="menu-link">من نحن</a>
                    <a href="#" class="menu-link">الهيكل التنظيمي</a>
                    <a href="#" class="menu-link">الهيكل الإستراتيجي للوزارة</a>
                    <a href="#" class="menu-link">السياسات والاستراتيجيات</a>
                    <a href="#" class="menu-link">أهداف التنمية المستدامة</a>
                    <a href="#" class="menu-link">الشركاء</a>
                    <a href="#" class="menu-link">الوظائف</a>
                    <a href="#" class="menu-link">تواصل معنا</a>
                    <a href="#" class="menu-link active">المشاركة الإلكترونية</a>
                    <a href="#" class="menu-link">الاستشارات</a>
                    <a href="#" class="menu-link">البيانات المفتوحة</a>
                     <a href="#" class="menu-link">التغذية الراجعة</a>
                      <a href="#" class="menu-link">التطوير المشترك والأفكار</a>
                       <a href="#" class="menu-link">وسائل التواصل الاجتماعي </a>
                       <h4>الأخبار والفعاليات</h4>
                    <a href="#" class="menu-link">الأخبار</a>
                     <a href="#" class="menu-link">الفعاليات</a>
                     <h4>المنافسات والميزانية</h4>
                      <a href="#" class="menu-link">المنافسات والمشتريات</a>
                       <a href="#" class="menu-link">الميزانية والإنفاق</a>
                   
                   
                   
                   
                   
                   
                </div>
            </div>
        </div>
    </details>
</div>

          
               
            
           <div class="menu">
    <details class="dropdown">
        <summary class="dropdown-title">مركز المعرفة</summary>
        <div class="dropdown-content">
            <div class="knowledge-section">
                
                
   
                <h2 class="section-title"></h2>
                <div class="links-list">
                    <h4>مبادرات وشراكات</h4>
                    <a href="#" class="menu-link">المبادرات</a>
                    <a href="#" class="menu-link">الشراكات</a>
                    <a href="#" class="menu-link">منصة استطلاع</a>
                    <a href="#" class="menu-link">منصة تفاعل</a>
                </div>

    <h4>بيانات وإحصائيات</h4>
                <h2 class="section-title"></h2>
                <div class="links-list">
                    <a href="#" class="menu-link">البيانات المفتوحة</a>
                    <a href="#" class="menu-link">الوثائق والتقارير</a>
                    <a href="#" class="menu-link">إحصائيات ومؤشرات المنصة</a>
                </div>
            </div>
        </div>
    </details>
</div>

            
            
            
            
            <div class="menu">
 
    <details class="dropdown">
        <summary class="dropdown-title">الخدمات</summary>
        <div class="dropdown-content">
            <div class="section">
                <h3>الصفحات الشخصية</h3>
                <a href="#">إدارة الطلبات</a>
                <a href="#">إدارة الرخص</a>
                <a href="#">لوحة التحكم <span class="new-badge">جديد</span></a>
            </div>
            
            <div class="section">
                <h3>المنظمات والأنظمة</h3>
                <a href="#">منصة رسم إشغال مرافق الإيواء</a>
                <a href="#">منصة رسم تقديم منتجات التبغ</a>
                <a href="#">بلدي أعمال <span class="new-badge">جديد</span></a>
                <a href="#">تصنيف مقدمي خدمات المدن</a>
            <h4>التفويض البلدي الإلكتروني</h4> 
             
             <a href="#" class="menu-link">إضافة منشأة إلى مدير حساب</a>
              <a href="#" class="menu-link">الاستعلام عن طلبات منشأة</a>
                   
      <a href="#" class="menu-link">الاستعلام عن مفوضي منشأة</a>
      
      <h4>الرخص التجارية</h4>
      
       <a href="#" class="menu-link">إصدار رخصة تجارية</a>
        <a href="#" class="menu-link">تجديد رخصة نشاط تجاري</a>
         <a href="#" class="menu-link">إلغاء رخصة نشاط تجاري </a>
         
         <h4>الرخص الإنشائية</h4>
         
          <a href="#" class="menu-link">إصدار رخصة بناء</a>
           <a href="#" class="menu-link">خدمة إصدار رخصة تسوير أراضي فضاء</a>
           
           <h4>الشهادات الصحية</h4>
           
            <a href="#" class="menu-link">إصدار شهادة صحية</a>
             <a href="#" class="menu-link">تجديد شهادة صحية</a>
             <h4>خدمات تنسيق المشروعات</h4>
              <a href="#" class="menu-link">خدمات تنسيق أعمال البنية التحتية</a>
           
            <a href="#" class="menu-link">خدمات تنسيق المشروعات الكبرى</a>
   
   <h4>خدمات التقارير المساحية</h4> 
    <a href="#" class="menu-link">إصدار تقرير مساحي</a>
          
          <h4>الهوية العقارية</h4>
          
          <br>
     
          
           <a href="#" class="menu-link">ربط صك إلكتروني بالهوية العقارية</a>
           
            <a href="#" class="menu-link"></a>
                   
           
                                                   
                   
                   
                        </div>
    </details>
</div>

                   
                   
                   
                   
                                   
                
      <div class="menu">
    <details class="dropdown">
        <summary class="dropdown-title">الاستعلامات</summary>
        <div class="dropdown-content">
            <div class="knowledge-section">
                
                
   
                <h4>الاستعلامات العامة</h4>
                
                <div class="links-list">
                    <a href="#" class="menu-link">الاستعلام عن المخالفة للإجراءات الاحترازية</a>
                    <a href="#" class="menu-link">حاسبة رسوم المعلوماتية </a>
                    <a href="#" class="menu-link">الاستعلام عن المكاتب الهندسية</a>
                    <a href="#" class="menu-link">الاستعلام عن عقود النظافة </a>
                    <a href="#" class="menu-link">أسواق المتاجر المتنقلة</a>
                    <a href="#" class="menu-link">الاستعلام عن  الإيقافات</a>
                    <a href="#" class="menu-link">الاستعلام عن المخالفات</a>
                    
                    <h4>الأراضي والبناء</h4>
                    
                     <a href="#" class="menu-link">الاستعلام عن رخصة بناء</a>
                   
                    
      
       <a href="#" class="menu-link">اشتراطات إيصال الخدمات الكهربائية </a>
       
            <a href="#" class="menu-link">المستكشف  الجغرافي</a>
                 
                  <a href="#" class="menu-link">مستكشف التغطية لخدمات البنية التحتية</a>
                  
                   <a href="#" class="menu-link">الاستعلام عن قرار مساحي</a>
             
             <h4>الاستعلامات التجارية</h4>   
              <a href="#" class="menu-link">استعلام عن رخصة نشاء تجاري</a>
               <a href="#" class="menu-link">الأنشطة التجارية والاشتراطات البلدية</a>
                <a href="#" class="menu-link">الاستعلام عن  مسارات العربات المتجولة</a>
                <h4>خدمات إكرام الموتى</h4>
                
     ‪ <a href="#" class="menu-link">الاستعلام عن مقدمي خدمات نقل وتجهيز الموتى (الجهات الخيرية)</a>
           
            <a href="#" class="menu-link">الاستعلام عن قبر متوفي</a>  
              
             <a href="#" class="menu-link">طباعة شهادة دفن</a>
              <a href="#" class="menu-link">الاستعلام عن المقابر</a>
              
               <a href="#" class="menu-link">الدليل التنظيمي للوحات البلدية</a>    
                   
                      
                   
                                     
      
       <a href="#" class="menu-link">اشتراطات إيصال الخدمات الكهربائية</a>
        <a href="#" class="menu-link">المستكشف الجغرافي</a>
         <a href="#" class="menu-link">مستكشف التغطية لخدمات البنية التحتية</a>
       
                </div>
            </div>
        </div>
    </details>
</div>
            
                       

    
    
    <div class="menu">
    <details class="dropdown">
        <summary class="dropdown-title">المنصات</summary>
        <div class="dropdown-content">
            <div class="knowledge-section">
                
                
   
                <h2 class="section-title"></h2>
                <div class="links-list">
                    
                    
                    <h5>بوابة الفرص الاستثمارية</h5>
                    <h5>المنصات التفاعلية</h5>
                </div>               
                
     <br>           
                
                </div>
            </div>
        </div>
    </details>
</div>
               
            <div class="menu">
    <details class="dropdown">
        <summary class="dropdown-title">تواصل معنا</summary>
        <div class="dropdown-content">
            <div class="knowledge-section">
                
                
   
                <h2 class="section-title"></h2>
                <div class="links-list">
                    <h5>اتصل بنا</h5>
                    <h5>بلاغ عن فساد</h5>
                    <h5>الأسئلة الشائعة</h5>
                    <h5>الدعم الفني بلغة الإشارة</h5>
                    <h5>دليل الأمانات</h5>
                    <h5>وسائل التواصل الاجتماعي</h5>
                    <h5>حجز موعد إلكتروني</h5>
                </div>

                </div>
            </div>
        </div>
    </details>
</div>
    
   
    <div class="container">
        <h1 class="title">الشهادة الصحية الموحدة</h1>   
        
      <img src="" alt="">
        
        <img src="https://i.ibb.co/ggjsBtd/Screenshot-20241031-180405.png"alt= "الصورة الشخصية" class="profile-photo">

        <div class="form-group">
            <div class="section-title">الامانة</div>
            <div class="form-value">أمانة منطقة حائل</div>
        </div>

        <div class="form-group">
            <div class="section-title">البلدية</div>
            <div class="form-value"> بلدية الوسط</div>
        </div>

        <div class="form-group">
            <div class="section-title">الاسم</div>
            <div class="form-value">حمزه محمد حميد احمد علي</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">رقم الهوية</div>
            <div class="form-value">2587238474</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">الجنس</div>
            <div class="form-value">ذكر</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">الجنسية</div>
            <div class="form-value">اليمن</div>
        </div>
    
        <div class="form-group">
            <div class="section-title">رقم الشهادة الصحية</div>
            <div class="form-value">400708239690</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">المهنة</div> 
            <div class="form-value">عامل تعبئة رفوف</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">تاريخ إصدار الشهادة الصحية هجري</div>
            <div class="form-value">1446/05/12</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">تاريخ إصدار الشهادة الصحية ميلادي</div>
            <div class="form-value">2024-11-14</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">تاريخ نهاية الشهادة الصحية هجري</div>
            <div class="form-value">1447/05/12</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">تاريخ نهاية الشهادة الصحية ميلادي</div>
            <div class="form-value">2025-11-14</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">نوع البرنامج التثقيفي</div>
            <div class="form-value">منشآت الغذاء</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">تاريخ انتهاء البرنامج التثقيفي</div>
            <div class="form-value">1449/04/03</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">رقم الرخصة</div>
            <div class="form-value">40011602597</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">اسم المنشأة</div>
            <div class="form-value">مطعم لذيذ للوجبات السريعة</div>
        </div>
        
        <div class="form-group">
            <div class="section-title">رقم المنشأة</div>
            <div class="form-value">7034376397</div>
        </div>


        <footer class="footer">
            <img src="https://i.ibb.co/X2jV205/Screenshot-20241025-150908.png" alt="Screenshot-20241025-150908" border="0" /></a>
            
            
            <div class="footer-text">© 2023 وزارة الشؤون البلدية والقروية والإسكان</div>
            <div class="footer-links">
                <a href="#">اتصل بنا</a>
                <a href="#">شروط الاستخدام</a>
                <a href="#">خريطة الموقع</a>
            </div>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Splash screen handling
            setTimeout(function() {
                const splash = document.querySelector('.splash-screen');
                splash.style.display = 'none';
            }, 2000);

            // Menu handling
            const menuIcon = document.querySelector('.menu-icon');
            const menuOverlay = document.querySelector('.menu-overlay');
            const body = document.body;

            menuIcon.addEventListener('click', function() {
                body.classList.toggle('menu-open');
            });

            menuOverlay.addEventListener('click', function() {
                body.classList.remove('menu-open');
            });
        });
                
    </script>
</body>
</html>

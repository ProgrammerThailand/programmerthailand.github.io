---
layout: post
title:  "Yii Framework 2 คืออะไร"
date:   2016-02-01 10:29:17 +0700
categories: Yii2Basic
author: "มานพ กองอุ่น"
---
หลายๆ เว็บไซต์ที่เราได้อ่านผ่านตาบ้างก็ค่อนข้างเชียร์กันยกใหญ่ว่า Yii Framework 2 นั้นมันเจ๋งนะ มันดีอย่างนั้น ดีอย่างนี้ ในบทความนี้เรามาดูกันว่า Yii Framework 2 นั้นมันคืออะไรกันแน่ ทำไมถึงได้มีคนนิยมชมชอบกันเยอะแยะเลยทีเดียว

ก่อนจะเป็น Yii Framework
---
ก่อนที่จะเป็น Yii Framework นั้นสมัยก่อนเวลาเราพัฒนา Web Application ด้วยภาษา PHP เราก็จะเขียนคำสั่งขึ้นมาเอง ถูกหลักบ้างผิดหลักบ้างแต่มันก็ออกมาเป็น Web Application นะ แต่ปัญหาที่เกิดขึ้นหลักๆ คือ เราเขียน คนอื่นๆ ไล่อ่านโค้ดนี่ปวดหัวเลย

ผ่านมาก็มีการเขียนโปรแกรมเชิงวัตถุหรือที่เรียกว่า Object Oriented Programming หรือ OOP เข้ามาก็ทำให้เกิดเป็นรูปแบบการเขียนที่หลากหลายขึ้น จึงมีคนกำหนดแนวคิดหนึ่งขึ้นมาเพื่อเป็นมาตรฐานในการแบ่งแยกการพัฒนาออกเป็นส่วนๆ เป็นการออกแบบสถาปัตยกรรมซอร์ฟแวร์แบบหนึ่ง เรียก  MVC หรือ Model View และ Controller นั่นเอง และได้รับความนิยมมาจนถึงปัจจุบัน

เมื่อมีเกณฑ์ดังกล่าวกำหนดขึ้นมาก็เกิด PHP Framework ต่างๆ ขึ้นมาที่ทำงานอยู่บนพื้นฐาน MVC เป็นต้นมานั่นเอง

ความหมายและที่มา
---
<div class="text-center">
<img src="/img/yii2basic/20160201/yii-logo.png" />
</div>
Yii หรือ ยี่ ย่อมาจาก Yes It Is เป็นเหมือนกับคำตอบหรือคำอุทานก็ว่าได้ที่ว่า มันเร็วจริงหรือเปล่า? มันมีความปลอดภัยไหม? มันมีความเป็นมืออาชีพหรือเปล่า? มันควรนำมาสร้าง Project ต่อไปหรือเปล่า? ใช่แล้วมันใช่จริงๆ (Yes It Is)

สำหรับ Yii นั้นเป็น Open Source ซึ่งเป็น PHP Framework สำหรับสร้าง Web Application ที่ถูกเขียนขึ้นให้รองรับ PHP5 ช่วยให้สร้าง Web Application ได้อย่างรวดเร็ว

Yii นั้นเกิดขึ้นจากคุณ Qiang Xue เป็นผู้ริเริ่ม Yii เมื่อ 1 มกราคม 2008 ซึ่งก่อนหน้าเขาเคยพัฒนา Prado Framework มาก่อนซึ่งก็มีประสบการณ์ต่างๆ มากกมาย และเห็นจุดอ่อนจุดแข็งของ Framework และได้นำประสบการณ์เหล่านั้นมาพัฒนาเป็น Yii Framework ในเวอร์ชั่นแรก

หลังจากนั้น Yii Framework ได้รับความนิยมเป็นอย่างมากในวงกว้างมากขึ้นเรื่อยๆ จนถึงปัจจุบัน ได้ออก Yii Framework ใน เวอร์ชั่น 2 ที่ Stable เรียบร้อยแล้วเมื่อวันที่ 12 ตุลาคม 2557 ที่ผ่านมา

แล้วทำไมต้องเป็น PHP Framework ล่ะ เขียน PHP ธรรมดาได้ไหม คำตอบคือ "ได้" แต่ว่าเราต้องเขียนทุกอย่างตั้งแต่เริ่มต้นจนเป็น Production โอ้แน่นอนครับต้องใช้เวลาในการเขียนโปรแกรมมากๆ เลยทีเดียว เหตุผลที่สำคัญอีกอย่างคือโปรแกรมเมอร์แต่ละคนเขียนโปรแกรมในแบบของตัวเองนี่สิ ทำให้ไม่มีมาตรฐานกลางเดียวกัน การไล่แก้โค้ดนั้นจะยากมาก



{% highlight php %}
<?php
    echo "Hello Yii Framework 2";
?>
{% endhighlight %}

Professional
---
Yii Framework 2 ออกแบบมาในรูปแบบ MVC หรือ Model View และ Controller ซึ่งเป็นการออกแบบสถาปัตยกรรมซอร์ฟแวร์แบบแบ่งชั้น และแน่นอนว่าเป็น Object Oriented Programming หรือ OOP 100%
โดย Yii Framework เป็นกลุ่มของ Class ที่เขียนขึ้นเพื่อช่วยให้เราสามารถพัฒนา Web Application ได้อย่างรวดเร็ว

Model คือตัวแทนของข้อมูล โดยใน Model จะมี Object Relation Mapping หรือ ORM ในการ Map Property ของ Class ให้เข้ากับ Attribute ของตาราง แบบอัตโนมัติ และยังมี Method ต่างๆ ที่ช่วยให้การทำงานกับข้อมูลได้สะดวกและรวดเร็วมากยิ่งขึ้น ตัวอย่างของ Model
{% highlight php %}
<?php
namespace common\models;
use yii\db\ActiveRecord;

class MyModel extends ActiveRecord{

    public static function tableName()
    {
        return 'table_name';
    }
    public function rules()
    {
        return [
            [['attribute1', 'attribute2'], 'required']
        ];
    }
    public function attributeLabels()
    {
        return [
            'attribute1' => 'Your Text1',
            'attribute2' => 'Your Text2'
        ];
    }
}
?>
{% endhighlight %}

View คือส่วนของการแสดงผล ใน Yii Framework 2 นั้นมี Widgets ต่างๆ ที่เข้ามาช่วยในการแสดงผลให้สามารถแสดงผลได้ตามต้องการ เช่น GridView จะแสดงข้อมูลออกมาในรูปแบบของตาราง ListView จะแสดงข้อมูลออกมาตาม template file ที่ต้องการได้ และ Detail View จะแสดงข้อมูลรายละเอียดในรายการข้อมูลที่เลือกได้ และมี Helpers ต่างๆ ที่เข้ามาช่วยในการแสดงผล เช่น Html helper เป็นตัวช่วยในการสร้างคำสั่ง html เช่น tag a, img เป็นต้น นอกจากจะแสดงผลแล้วยังมีส่วนของความปลอดภัยร่วมด้วย
{% highlight php %}
<?php
use yii\helpers\Html;
use yii\widgets\DetailView;
use yii\grid\GridView;
use yii\widgets\ListView;

echo DetailView::widget([
    'model' => $model
]);

echo GridView::widget([
    'dataProvider' => $dataProvider
]);

echo ListView::widget([
    'dataProvider' => $dataProvider,
    'itemView' => '_item_template' //item template file
]);
?>
{% endhighlight %}

Controller คือส่วนของการควบคุมการทำงานระหว่าง Model และ View เป็นส่วนหลักของ Logic Program
{% highlight php %}
<?php
namespace frontend\controllers;

use Yii;
use yii\web\Controller;
use common\models\Property;

class PropertyController extends Controller
{
    public function actionIndex()
    {
        $query = Property::find();

        $request = Yii::$app->request;

        $type = $request->get('type');
        $property_type = $request->get('property_type');
        $address = $request->get('address');

        $dataProvider = new ActiveDataProvider([
            'query' => $query,
            'sort' => [
                'defaultOrder' => [
                    'id' => SORT_DESC
                ]
            ]
        ]);

        $query->andFilterWhere(['like', 'property_status', $type])
            ->andFilterWhere(['like', 'address', $address])
            ->andFilterWhere(['like', 'property_type_id', $property_type]);

        $count_item = $query->count();
        return $this->render('index', [
            'dataProvider' => $dataProvider,
            'count_item' => $count_item,
        ]);
    }
}

?>
{% endhighlight %}

Performance
---
Yii Framework 2 มีประสิทธิภาพในเรื่องของการทำ Caching เพื่อเพิ่มประสิทธิภาพด้านการประมวลผลที่รวดเร็วมากยิ่งขึ้น การทำ RBAC หรือ Role Base Access Control ซึ่งช่วยในการจัดการสิทธิ์ในการเข้าถึงในระดับ Action ได้เลย เป็นต้น

ส่วนในด้านของการพัฒนา Yii Framework 2 มีตัวช่วยในการ Generate Code ที่ชื่อว่า Gii Generator ซึ่งเป็นตัวช่วยที่สำคัญในการเขียนโปรแกรม โดยมีขั้นตอนง่ายๆ ในการพัฒนา Web Application ของคุณคือ
1. System Analysis วิเคราะห์และออกแบบระบบให้ได้ฐานข้อมูล
2. Generate Code ด้วย Gii เพื่อให้ได้คำสั่งพื้นฐานและโครงสร้างของระบบ เช่น Create Read Update และ Delete หรือ CRUD
3. แก้ไขโปรแกรมให้เข้ากับความต้องการ

เพียง 3 ขั้นตอนนี้ก็สามารถพัฒนา Web Application ได้อย่างง่ายดายแล้ว

Security
---
ในด้านของความปลอดภัยใน Yii Framework 2 มีตัวช่วยด้านความปลอดภัยมาให้เช่น CSRF หรือ Cross-site script forgery ที่มีให้แบบอัตโนมัติทุกครั้งที่มีการสร้างฟอร์มด้วย ActiveForm
มีการป้องกันจาก XSS หรือ Cross-site scripting ที่จะดึงข้อมูลจากฐานข้อมูลมาแสดงผลด้วย HTML helpers และ HTMLPurifier เช่น Html::encode() และ HtmlPurifier::process() และความปลอดภัยด้านการป้องกันจาก SQL Injection ก็ยังมีมาให้ในตัวอีกด้วย เรียกได้ว่ามาแบบครบเครื่องเลยทีเดียวครับ

{% highlight php %}
<?php
use yii\helpers\Html;
use yii\helpers\HtmlPurifier;

echo Html::encode($model->title);
echo HtmlPurifier::process($model->description);
?>
{% endhighlight %}

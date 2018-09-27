---
layout: tour
title: บทนำ

discourse: false

partof: scala-tour

num: 1

language: th

next-page: basics
---

## ยินดีต้อนรับสู่การเดินทาง
การเดินทางครั้งนี้ประกอบด้วยการแนะนำแบบสั้นๆ สำหรับแต่ล่ะคุณสมบัติของ Scala ที่ใช้บ่อยที่สุด และมีมีความตั้งใจเพื่อสำหรับผู้ที่เรียนรู้ภาษา Scala ใหม่

และนี่ก็เป็นเพียงบทความสั้นๆ ที่ไม่ใช้การสอนเต็มรูปแบบของภาษา Scala หากต้องการเรียนรู้มากขึ้นให้พิจารณา[หนังสือ](/books.html) หรือขอคำปรึกษาจาก[แหล่งอื่นๆ](/learn.html)

## อะไรคือ Scala?
 Scala เป็นภาษาเขียนโปรแกรมแบบหลากหลายกระบวนทัศน์ที่ทันสมัย ที่ออกแบบมาเพื่อแสดงรูปแบบการเขียนโปรแกรมโดยทั่วไปที่กระชับ สง่างาม และมีชนิดข้อมูลที่ปลอดภัย (type-safe) ซึ่งผสานคุณสมบัติของภาษาเชิงวัตถุและภาษาเชิงฟังก์ชัน

## Scala เป็นภาษาเชิงวัตถุ ##
Scala เป็นภาษาการเขียนโปรแกรมเชิงวัตถุที่แท้จริง ในแง่ที [่ทุกค่าเป็นวัตถุ](unified-types.html) ชนิดข้อมูลและพฤติกรรมของวัตถุอธิบายโดย[คลาส (classes)](classes.html) และ [ลักษณะ (traits)](traits.html) คลาสจะถูกขนายโดยการจัดชั้นย่อย (subclassing) และกลไล[องค์ประกอบแบบผสมผสาน (mixin-based composition)](mixin-class-composition.html) ที่มีความยืดหยุ่นเพื่อทดแทนสำหรับการสืบทอดหลายแบบ

## Scala เป็นภาษาเชิงฟังก์ชัน ##
Scala ยังเป็นภาษาเชิงฟังก์ชันในแง่ที่ [ทุกฟังก์ชันเป็นค่า](unified-types.html)  Scala มี[ไวยกรณ์แบบง่าย](basics.html#functions)สำหรับกำหนดฟังก์ชันที่ไม่ระบุตัวตน รองรับ [ฟังก์ชันที่มีลำดับสูงขึ้น (higher-order functions)](higher-order-functions.html) ทำให้ฟังก์ชันสามารถ [ซ้อนกันได้ (nested)](nested-functions.html) และรองรับ [currying](multiple-parameter-lists.html), [เคสคลาส (case class)](case-classes.html) ของ Scala สนับสนุน [รูปแบบการจับคู่ (pattern-matching)](pattern-matching.html) เป็นการจำลองชนิดข้อมูลแบบพีชคณิตที่ใช้ในภาษาเชิงฟังก์ชันหลายภาษา, [วัตถุ Singleton](singleton-objects.html) ทำให้มีวิธีที่สะดวกในการจัดกลุ่มฟังก์ชันที่ไม่ใช้สมาชิกของคลาส

นอกจากนี้ Scala มีแนวคิดของรูปแบบการจับคู่โดยธรรมชาติซึ่งสามารถขยายเป็น [การประมวลผลข้อมูลด้วย XML](https://github.com/scala/scala-xml/wiki/XML-Processing) ด้วยความช่วยเหลือของ [รูปแบบลำดับที่ถูกละเลย (right-ignoring sequence patterns)](regular-expression-patterns.html), โดยวิธีของการขยายทั่วไปผ่านทาง [วัตถุตัวดึงข้อมูล (extractor object)](extractor-objects.html) ในบริบทนี้ การ[ทำความเข้าใจ for](for-comprehensions.html) มีประโยชน์สำหรับการคิดสูตรคิวรี่ข้อมูล คุณลักษณะเหล่านี้ทำให้ Scala เหมาะสำหรับการพัฒนาแอพพลิเคชันแบบเช่นเว็บเซอร์วิส

## Scala มีชนิดข้อมูลแบบคงที่ ##
Scala เป็นระบบที่มีลักษณะของชนิดข้อมูลบังคับให้เป็นแบบคงที่ (statically) ว่าสิ่งที่เป็นนามธรรม (abstraction) ถูกใช้อย่างปลอดภัยและสอดคล้องกัน โดยเฉพาะอย่างยิ่ง ระบบชนิดข้อมูลสนับสนุนข้อมูลหลายประเภท ดังนี้:

* [คลาสทั่วไป](generic-classes.html)
* [คำอธิบายประกอบผันแปร](variances.html)
* ขอบเขตชนิดข้อมูล [ข้างบน](upper-type-bounds.html) และ [ข้างล่าง](lower-type-bounds.html)
* [คลาสภายใน](inner-classes.html) และ [ชนิดข้อมูลนามธรรม](abstract-types.html) เป็นสมาชิกของวัตถุ
* [ชนิดข้อมูลผสม](compound-types.html)
* [อ้างอิงตัวเองของชนิดข้อมูลอย่างชัดเจน](self-types.html)
* [พารามิเตอร์ปริยาย](implicit-parameters.html) และ [การเปลี่ยนปริยาย](implicit-conversions.html)
* [เมธอดหลายรูปแบบ)](polymorphic-methods.html)

[ชนิดข้อมูลอนุมาน (Type inferrence)](type-inference.html) หมายถึงผู้ใช้ไม่จำเป็นต้องใส่โค้ดคำอธิบายประกอบที่มีข้อมูลซ้ำซ้อน ในการรวม คุณสมบัติเหล่านี้จะเป็นคุณสมบัติพื้นฐานที่มีประสิทธิภาพสำหรับการนำส่วนของโปรแกรมที่เป็นนามธรรม มาใช้ใหม่ได้อย่างปลอดภัยและเพื่อให้สามารถขยาย ชนิดข้อมูลที่ปลอดภัยของซอฟต์แวร์

## Scala สามารถขยายออกได้ ##

ในทางปฏิบัต การพัฒนาแอพพลิเคชันเฉพาะโดเมนมักต้องใช้ส่วนขยายของภาษาเฉพาะโดเมน ซึ่ง Scala มีการรวบรวมกลไกเฉพาะที่ทำให้ง่ายต่อการเพิ่มโครงสร้างภาษาใหม่ ในรูปแบบห้องสมุด

ในหลายกรณีสามารถทำได้โดยไม่ปราศจากสิ่งอำนวยความสะดวกเมตาดาต้าโปรแกรม อย่างเช่น มาโคร, ตัวอย่างเช่น

* [คลาสโดยปริยาย](http://docs.scala-lang.org/overviews/core/implicit-classes.html) อนุญาติให้เพิ่มขยายเมธอดกับชนิดข้อมูลที่มีอยู่
* [สอดแทรกสตริงตัวอักษร](/overviews/core/string-interpolation.html) คือการขยายโดยผู้ใช้ด้วยตัวสอดแทรกที่กำหนดเอง.

## Scala ทำงานร่วมกันได้

Scala ออกแบบมาเพื่อให้ทำงานร่วมกันกับ Java Runtime Environment (JRE) โดยเฉพาะอย่างยิ่งปฏิสัมพันธ์กับหลักภาษาโปรแกรมเชิงวัตถุ Java อย่างราบรื่นไร้รอยต่อ คุณสมบัติใหม่ของภาษา Java อย่างเช่น SAMs, [Lambdas](higher-order-functions.html), [annotations](annotations.html) และ [generics](generic-classes.html) มีความคล้ายคลึงกับ Scala

คุณสมบัติเหล่านี้ของ Scala ที่ไม่คล้ายคลึงกับ Java อย่างเช่น [default](default-parameter-values.html) และ [ชื่อพารามิเตอร์](named-arguments.html) จะถูกคอมไพล์ให้ใกล้เคียงกับ Java ตามที่สมควร ซึ่ง Scala มีการคอมไพล์แบบเดียวกันกับ Java (แยกการคอมไพล์, การโหลดคลาสแบบไดนามิก) ทำให้สามารถเข้าถึงไลบรารี่ที่มีคุณภาพสูงของ Java จำนวนมากได้

## ขอให้สนุกกับการเดินทาง!

ไปต่อได้ที่ [หน้าถัดไป](basics.html) ในเมนูของเนื้อหาเพื่ออ่านเพิ่มเติม
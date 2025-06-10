# ⚽️ طبقه‌بندی پست بازیکنان فوتبال با مدل CLIP

این پروژه با استفاده از مدل بینایی CLIP پیاده‌سازی شده است. هدف، طبقه‌بندی تصویر بازیکن فوتبال به یکی از ۴ پست زیر است:

- دروازه‌بان
- مدافع
- هافبک
- مهاجم

## 📌 مراحل انجام‌شده

1. دریافت دیتاست از کوئرا  
   🔗 [لینک سوال و دیتاست](https://quera.org/problemset/292199?tab=description)

2. پیش‌پردازش داده‌ها با استفاده از Albumentations و ساخت DataLoader

3. استفاده از بخش بینایی مدل CLIP به‌عنوان استخراج‌کننده ویژگی 

4. طراحی مدل طبقه‌بند شامل چند لایه `Linear` و `ReLU`

5. پیاده‌سازی حلقه آموزش با ثبت دقت و لا‌س روی `train` و `validation`

6. کاهش هوشمند learning rate با استفاده از ReduceLROnPlateau

7. ذخیره بهترین وزن‌های مدل با نام `best_model.pth`

8. پیاده‌سازی تابع `predict` برای پیش‌بینی پست بازیکنان در تصاویر تست

9. رسم نمودارهای loss و accuracy در پایان آموزش


# ⚽️ Football Player Position Classification with CLIP

This project uses the vision part of OpenAI's CLIP model to classify football players into 4 positions based on their images:

- Goalkeeper
- Defender
- Midfielder
- Forward

## ✅ Steps Done

1. Download dataset from Quera  
   🔗 [Link to problem & dataset](https://quera.org/problemset/292199?tab=description)

2. Preprocess data using Albumentations and setup DataLoaders

3. Use CLIP vision model 

4. Build a classifier with several `Linear` and `ReLU` layers

5. Implement training loop with accuracy/loss logging on train and validation

6. Add ReduceLROnPlateau to adjust learning rate dynamically

7. Save the best model weights to `best_model.pth`

8. Implement `predict` function for test set inference

9. Plot training/validation accuracy and loss per epoch


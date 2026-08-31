# `studio/` — غیرریپو

دو شاخه، دو عمر متفاوت:

```
studio/
  archive/     منجمد: پروژهٔ مرده + بسته/دامپ
  desk/        زنده: دانش + عملیات روزانه
```

ریپوی فعال اینجا نیست → `~/dev/personal` یا `~/dev/work`.

## کجا بگذارم؟

```
فایل جدید
  ├─ هنوز نمی‌دانی؟                    → desk/inbox/
  ├─ راز / کلید / recovery / SSH       → desk/config/   (هرگز git)
  ├─ «چطور deploy/عیب‌یابی کنم؟»        → desk/runbooks/
  ├─ compose / env / بستهٔ سرور        → desk/deploy/<سرویس>/
  ├─ حادثه با زمان و اقدام             → desk/incidents/
  ├─ قالب تکرارشونده (seed, compose)   → desk/templates/
  ├─ یادداشت خام برای چسباندن به LLM   → desk/llm/
  ├─ تصویر/اسکرین                    → desk/media/
  ├─ یادگیری / PDF / مرجع کوتاه        → desk/knowledge/
  ├─ کد/پروژهٔ مرده                    → archive/projects/<نام>/
  └─ zip، دامپ DB، docker save، خروجی  → archive/artifacts/…
```

## قانون نام‌گذاری

- kebab-case، بدون فاصله در نام پوشه
- دامپ تاریخ‌دار: `YYYY-MM-DD-موضوع`
- یک README فقط برای ساختار؛ محتوای پروژه را اینجا توضیح نده

## symlinkهای `~/dev`

`archive` → اینجا؛ `configs` → `desk/config`؛ `DevOps` → `desk/runbooks`.

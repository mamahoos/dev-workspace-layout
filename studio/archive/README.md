# `archive/` — منجمد

ریشه باید خلوت بماند. فقط دو درخت + یک symlink سازگاری:

```
archive/
  projects/     درخت سورس/پروژهٔ قدیمی (دست‌نخورده بماند مگر بدانی)
  artifacts/    بسته، دامپ، خروجی ابزار، اسکریپت پراکنده
  docker-images → artifacts/container-images/docker-images
```

کد داخل `projects/programing` را جابه‌جا نکن؛ نام تاریخی `programing` عمداً مانده.

پروژهٔ جدیدِ مرده: `projects/<kebab-name>/`  
بستهٔ همان پروژه: `artifacts/archives/projects/` یا اگر مال یک پوشه است `_artifacts/` داخل همان پروژه (پایین).

## الگوی `_artifacts` داخل یک پروژه

```
projects/<نام>/
  _artifacts/
    archives/
    databases/
    exports/
    images/
```

فقط zip/tar/دامپ/docker-save. venv و سورس را منتقل نکن.

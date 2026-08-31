> این ریپو **فقط** نقشهٔ پوشه‌بندی `~/dev` است (فایل‌های `README.md` ساختار). سورس، بکاپ، و راز اینجا نیستند.

# `~/dev`

فضای کار نرم‌افزار. هر چیز در یکی از چهار ریشه است؛ مسیرهای قدیمی با symlink حفظ شده‌اند.

| مسیر | نقش | چه چیزی اینجا می‌آید |
| --- | --- | --- |
| `personal/` | ریپوهای فعال خودت (`mamahoos`) | پروژهٔ در حال کار، با `.git` |
| `work/` | کار شرکت | عمداً جدا از personal |
| `vendor/` | clone دیگران | upstream ≠ mamahoos |
| `studio/` | غیرریپو: آرشیو + میزکار | دانش، عملیات، بکاپ، کد مرده |

جزئیات studio: [`studio/README.md`](studio/README.md)

## سازگاری مسیر (دست نزن)

این سه نام در ریشهٔ `~/dev` باید بمانند:

| symlink | هدف |
| --- | --- |
| `archive` | `studio/archive` |
| `configs` | `studio/desk/config` |
| `DevOps` | `studio/desk/runbooks` |

داخل archive: `docker-images` → `artifacts/container-images/docker-images`

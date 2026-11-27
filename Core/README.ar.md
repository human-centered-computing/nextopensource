# Core — الأساس المشترك للمصدر المفتوح

[English](README.md) · [Türkçe](README.tr.md) · [Deutsch](README.de.md) · [العربية](README.ar.md)

[NextOpenSource](../README.ar.md)

الدليل وموقع مصدر المكونات القابلة لإعادة الاستخدام من المشاريع الأصلية لـ HCC. لكل مكون معتمد مجلد ثابت `Core/<ComponentID>/`.

```text
Core/
  README.md
  README.tr.md
  <ComponentID>/                 # one directory per upstream component
    README.md                    # origin, purpose, pinned version, use
    README.tr.md                 # Turkish
    README.de.md                 # German
    README.ar.md                 # Arabic
    UPSTREAM.md                  # provenance and review record
    source/                      # authorized upstream source snapshot or Git submodule
    patches/                     # explicitly recorded HCC changes, if required
```

## قواعد الاستيراد والصيانة
- قبل الاستيراد سجل عنوان الأصل والالتزام أو الوسم والترخيص والإشعارات والصيانة والتبعيات ومراجعة الأمن والاستخدام والموافقة البشرية. [القالب](../templates/UPSTREAM.md).
- احفظ التراخيص والنسب والمنشأ الأصلي. استخدم إصداراً مثبتاً ومتحققاً، أو مستودع Core مستقل أو وحدة فرعية دون تكرار. تتبع تغييرات HCC منفصلة.
- لا بيانات منتج موطنة أو أسرار أو موارد عرض أو شفرة مملوكة في الأساس الأصلي؛ تبقى التكييفات في المنتج والرقع اللازمة موثقة ومراجعة منفصلة.
- تحقق من التحديث والترخيص والأمن واربط اختبارات NextSecurity. لا تستورد منشأ أو ترخيصاً غير واضح ولا تفترض ترخيصاً لمجرد الخصوصية.
- خطط التقييم والتكامل في مجلد المشروع في NextOpenSource وNextRoadmap، واستخدم المكتبة المشتركة دون نسخ لكل مشروع.

## المكونات
| المكون | الأصل | الإصدار | الترخيص | الحالة |
|---|---|---|---|---|
| [NextID-Core](NextID-Core/README.md) | [Keycloak](https://github.com/keycloak/keycloak) | [`26.8.2`](https://github.com/keycloak/keycloak/commit/e514445f9dcdabc5bdcf67cab56c1e49655de067) | Apache-2.0 | نسخة مصدر كاملة غير معدلة؛ تحقق الأمن والبناء معلق |

أضف مكونات أخرى بعد المراجعة والتفويض.
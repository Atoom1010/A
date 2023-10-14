{
    "name": {
        "ar": "قوالب العنايه والجمال",
        "en": "beauty"
    },
    "repository": "https://github.com/Atoom1010/beauty",
    "author_email": "atooomy22222@gmail.com",
    "features": [
        "mega-menu",
        "fonts",
        "color",
        "breadcrumb",
        "unite-cards-height",
        "component-featured-products",
        "component-fixed-banner",
        "component-fixed-products",
        "component-products-slider",
        "component-photos-slider",
        "component-parallax-background",
        "component-testimonials",
        "component-square-photos",
        "component-store-features",
        "component-youtube"
    ],
    "settings": [
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "وضع عمودي للمنتجات في مربع المنتجات الثابتة في الصفحة الرئيسية",
            "description": null,
            "id": "vertical_fixed_products",
            "format": "switch",
            "required": false,
            "value": false,
            "selected": false
        },
        {
            "type": "boolean",
            "id": "is_more_button_enabled",
            "label": "عرض (زر الكل) في الصفحة الرئيسية",
            "format": "switch"
        },
        {
            "type": "static",
            "id": "static-line1",
            "format": "line"
        },
        {
            "type": "static",
            "format": "title",
            "id": "static-label2",
            "value": "خيارات أعلى الصفحة",
            "variant": "h6"
        },
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "شريط علوي داكن",
            "description": null,
            "id": "topnav_is_dark",
            "format": "switch",
            "required": false,
            "value": true,
            "selected": false
        },
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "عرض روابط الصفحات الهامة في الشريط العلوي",
            "description": "مثل صفحة الهبوط ، المدونة ،الصفحات التعريفية",
            "id": "important_links",
            "format": "switch",
            "required": false,
            "value": true,
            "selected": true
        },
        {
            "type": "static",
            "id": "static-line3",
            "format": "line"
        },
        {
            "type": "static",
            "format": "title",
            "id": "static-label4",
            "value": "خيارات أسفل الصفحة",
            "variant": "h6"
        },
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "الوضع الداكن",
            "description": null,
            "id": "footer_is_dark",
            "format": "switch",
            "required": false,
            "value": true,
            "selected": false
        },
        {
            "type": "static",
            "id": "static-line5",
            "format": "line"
        },
        {
            "type": "static",
            "format": "title",
            "id": "static-label6",
            "value": "خيارات صفحة المنتج",
            "variant": "h6"
        },
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "تثبيت زر الإضافة والكمية أسفل شاشة الجوال",
            "description": null,
            "id": "sticky_add_to_cart",
            "format": "switch",
            "required": false,
            "value": true,
            "selected": true
        },
        {
            "type": "boolean",
            "icon": "sicon-toggle-off",
            "label": "اظهار الوسوم",
            "description": null,
            "id": "show_tags",
            "format": "switch",
            "required": false,
            "value": true,
            "selected": true
        },
        {
            "id": "slider_background_size",
            "type": "items",
            "format": "dropdown-list",
            "label": "طريقة عرض الصور في سليدر صور المنتج",
            "description": null,
            "labelHTML": null,
            "icon": "sicon-list",
            "selected": [
                {
                    "label": "اظهار الصورة كاملةً في المنتصف (Contain)",
                    "value": "contain",
                    "key": "f4adec13-6e4c-433b-b141-b2807935ced9"
                }
            ],
            "options": [
                {
                    "label": "تغطية الصورة كامل المساحة مع المحافظة على النسبة الصورة (Cover)",
                    "value": "cover",
                    "key": "e9c8ea8f-c5c6-438e-9d45-3bce269afde4"
                },
                {
                    "label": "اظهار الصورة كاملةً في المنتصف (Contain)",
                    "value": "contain",
                    "key": "f4adec13-6e4c-433b-b141-b2807935ced9"
                }
            ],
            "source": "Manual",
            "required": true
        }
    ],
    "components": [
        {
            "key": "186b3f4f-25cf-4d3c-abca-cef7eed6f0ab",
            "title": "صور متحركة (محسنة)",
            "icon": "sicon-image-carousel",
            "path": "home.enhanced-slider",
            "fields": [
                {
                    "type": "static",
                    "format": "description",
                    "id": "static-desc",
                    "value": "<div ><h6 >معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/main-slider.jpg?v=1.1'></div>"
                },
                {
                    "type": "static",
                    "format": "description",
                    "id": "static-note",
                    "value": "<h4 >هذا العنصر غير مناسب لعرض البنرات، يمكنك استخدام عنصر <strong>صور متحركة</strong> بدلاً من عنصر <strong>صور متحركة محسنة</strong> لتظهر صورة البنر بشكل كامل</h4>"
                },
                {
                    "id": "slides",
                    "type": "collection",
                    "format": "collection",
                    "required": true,
                    "minLength": 1,
                    "maxLength": 10,
                    "label": null,
                    "item_label": "صورة",
                    "value": [],
                    "fields": [
                        {
                            "type": "string",
                            "icon": "sicon-image",
                            "value": null,
                            "id": "slides.image",
                            "label": "صورة البنر",
                            "format": "image",
                            "required": true,
                            "placeholder": null,
                            "description": "* المقاس المناسب للصورة هو 900×600 بكسل"
                        },
                        {
                            "type": "string",
                            "icon": "sicon-format-text-alt",
                            "label": "عنوان رئيسي",
                            "multilanguage": true,
                            "id": "slides.title",
                            "value": null,
                            "required": false,
                            "format": "text",
                            "description": "يتم عرضه على الصورة بحجم بارز جداً، مع إضافة تأثير دخول للنص يضيف لمسة جمالية على معرض الصور.",
                            "placeholder": "يمكنك إضافة عنوان بارز هنا...",
                            "hide": false,
                            "minLength": 0,
                            "maxLength": 100
                        },
                        {
                            "type": "string",
                            "icon": "sicon-typography",
                            "label": "نص إضافي",
                            "multilanguage": true,
                            "id": "slides.description",
                            "value": null,
                            "description": "يتم عرضه على الصورة بحجم أصغر من العنوان الرئيسي، مع إضافة تأثير دخول للنص يضيف لمسة جمالية على معرض الصور.",
                            "format": "textarea",
                            "required": false,
                            "placeholder": "يمكنك إضافة تفاصيل إضافية هنا",
                            "minLength": 0,
                            "maxLength": 255
                        }
                    ]
                }
            ]
        },
        {
            "key": "2b1b130b-5b37-422a-9683-e0fd367460c0",
            "title": "روابط سريعة",
            "icon": "sicon-layout-grid-rearrange",
            "path": "home.main-links",
            "fields": [
                {
                    "type": "static",
                    "format": "description",
                    "id": "with-bg",
                    "value": "<div style='padding-top:10px;margin-bottom:30px;border:1px solid #ebebeb;border-radius:5px;text-align:center;overflow:hidden'><h6 style='margin-bottom:10px'>معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/main-links-with-bg.jpg?v=1.1'></div>",
                    "conditions": [
                        {
                            "id": "merge_with_top_component",
                            "operation": "=",
                            "value": true
                        }
                    ]
                },
                {
                    "type": "static",
                    "format": "description",
                    "id": "without-bg",
                    "value": "<div style='padding-top:10px;margin-bottom:30px;border:1px solid #ebebeb;border-radius:5px;text-align:center;overflow:hidden'><h6 style='margin-bottom:10px'>معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/main-links.png?v=1.1'></div>",
                    "conditions": [
                        {
                            "id": "merge_with_top_component",
                            "operation": "=",
                            "value": false
                        }
                    ]
                },
                {
                    "type": "string",
                    "icon": "sicon-format-text-alt",
                    "label": "العنوان",
                    "multilanguage": true,
                    "id": "title",
                    "value": null,
                    "required": false,
                    "format": "text",
                    "description": null,
                    "placeholder": "أدخل العنوان هنا...",
                    "minLength": 0,
                    "maxLength": 100
                },
                {
                    "type": "boolean",
                    "icon": "sicon-toggle-off",
                    "label": "دمج مع العنصر السابق",
                    "description": null,
                    "id": "merge_with_top_component",
                    "format": "switch",
                    "required": false,
                    "value": false,
                    "selected": false
                },
                {
                    "type": "boolean",
                    "icon": "sicon-toggle-off",
                    "label": "عرض أسهم التحرك",
                    "description": "",
                    "id": "show_controls",
                    "format": "switch",
                    "required": false,
                    "value": true,
                    "selected": true
                },
                {
                    "type": "static",
                    "format": "description",
                    "id": "static-desc",
                    "value": "<small >* إزاحة كامل العنصر ومحتوياته مع العنصر السابق، وجعلهما يظهران كعنصر واحد متناسق، يكون ذا فائدة في حالة كان العنصر السابق هو (صور متحركة محسنة). </small>"
                },
                {
                    "id": "links",
                    "type": "collection",
                    "format": "collection",
                    "required": true,
                    "minLength": 3,
                    "maxLength": 100,
                    "item_label": "رابط ",
                    "value": [
                        {
                            "links.icon": "sicon-store2",
                            "links.url__type": "offers_link"
                        },
                        {
                            "links.icon": "sicon-shopping-bag",
                            "links.url__type": "offers_link"
                        },
                        {
                            "links.icon": "sicon-favorite",
                            "links.url__type": "offers_link"
                        }
                    ],
                    "fields": [
                        {
                            "type": "string",
                            "icon": "sicon-format-text-alt",
                            "label": "عنوان الرابط",
                            "id": "links.icon",
                            "value": "sicon-store2",
                            "required": true,
                            "format": "icon",
                            "description": null
                        },
                        {
                            "type": "string",
                            "icon": "sicon-format-text-alt",
                            "multilanguage": true,
                            "id": "links.title",
                            "value": null,
                            "required": true,
                            "format": "text",
                            "description": null,
                            "placeholder": "أدخل عنوان للرابط هنا...",
                            "minLength": 2,
                            "maxLength": 80
                        },
                        {
                            "type": "items",
                            "icon": "sicon-link",
                            "label": "الرابط",
                            "id": "links.url",
                            "value": null,
                            "description": null,
                            "required": false,
                            "format": "variable-list",
                            "searchable": true,
                            "source": "custom",
                            "sources": [
                                {
                                    "label": "منتج",
                                    "key": "products",
                                    "value": "products"
                                },
                                {
                                    "label": "تصنيف",
                                    "key": "categories",
                                    "value": "categories"
                                },
                                {
                                    "label": "ماركة تجارية",
                                    "key": "brands",
                                    "value": "brands"
                                },
                                {
                                    "label": "صفحة تعريفية",
                                    "key": "pages",
                                    "value": "pages"
                                },
                                {
                                    "label": "مقالة",
                                    "key": "blog_articles",
                                    "value": "blog_articles"
                                },
                                {
                                    "label": "تصنيف ضمن المدونة",
                                    "key": "blog_categories",
                                    "value": "blog_categories"
                                },
                                {
                                    "label": "التخفيضات",
                                    "key": "offers_link",
                                    "value": "offers_link"
                                },
                                {
                                    "label": "الماركات التجارية",
                                    "key": "brands_link",
                                    "value": "brands_link"
                                },
                                {
                                    "label": "المدونة",
                                    "key": "blog_link",
                                    "value": "blog_link"
                                },
                                {
                                    "label": "رابط خارجي",
                                    "key": "custom",
                                    "value": "custom"
                                }
                            ]
                        }
                    ]
                }
            ]
        },
        {
            "key": "25f6cf26-a53f-4954-9b32-739b311b32c7",
            "title": "الماركات التجارية",
            "icon": "sicon-award-ribbon",
            "path": "home.brands",
            "fields": [
                {
                    "type": "static",
                    "format": "description",
                    "id": "with-bg",
                    "value": "<div style='padding-top:10px;margin-bottom:30px;border:1px solid #ebebeb;border-radius:5px;text-align:center;overflow:hidden'><h6 style='margin-bottom:10px'>معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/brands.jpg?v=1.1'></div>"
                },
                {
                    "type": "string",
                    "icon": "sicon-format-text-alt",
                    "label": "العنوان",
                    "multilanguage": true,
                    "id": "title",
                    "required": false,
                    "format": "text",
                    "description": "",
                    "placeholder": "أدخل العنوان هنا...",
                    "minLength": 0,
                    "maxLength": 200,
                    "value": {
                        "ar": "تصفح من خلال العلامات التجارية",
                        "en": "Browse All Brands"
                    }
                },
                {
                    "type": "items",
                    "icon": "sicon-keyboard_arrow_down",
                    "label": "الماركات التجارية",
                    "id": "brands",
                    "format": "dropdown-list",
                    "description": "",
                    "selected": [],
                    "options": [],
                    "required": true,
                    "multichoice": true,
                    "searchable": true,
                    "source": "brands"
                }
            ]
        },
        {
            "key": "9a758d20-2ce4-4782-91fe-c04466464588",
            "title": "منتجات متحركة مع خلفية",
            "icon": "sicon-list-play",
            "path": "home.slider-products-with-header",
            "fields": [
                {
                    "type": "static",
                    "format": "description",
                    "id": "with-bg",
                    "value": "<div style='padding-top:10px;margin-bottom:30px;border:1px solid #ebebeb;border-radius:5px;text-align:center;overflow:hidden'><h6 style='margin-bottom:10px'>معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/product-slider-with-header-bg.jpg?v=1.1'></div>"
                },
                {
                    "type": "string",
                    "icon": "sicon-image",
                    "value": null,
                    "label": "صورة الخلفية",
                    "id": "background",
                    "format": "image",
                    "required": true,
                    "placeholder": "",
                    "description": "* المقاس المناسب للصورة هو 1233×500 بكسل",
                    "settings": {
                        "height": 427,
                        "width": 640
                    }
                },
                {
                    "type": "string",
                    "icon": "sicon-format-text-alt",
                    "label": "عنوان رئيسي",
                    "multilanguage": true,
                    "id": "title",
                    "value": null,
                    "required": false,
                    "format": "text",
                    "description": "",
                    "placeholder": "يمكنك إضافة العنوان الرئيسي هنا...",
                    "hide": false,
                    "minLength": 0,
                    "maxLength": 80
                },
                {
                    "type": "string",
                    "icon": "sicon-typography",
                    "label": "نص توضيحي",
                    "multilanguage": true,
                    "id": "description",
                    "value": null,
                    "description": "",
                    "format": "textarea",
                    "required": false,
                    "placeholder": "يمكنك إضافة وصف لهذا القسم هنا...",
                    "minLength": 0,
                    "maxLength": 255
                },
                {
                    "type": "items",
                    "icon": "sicon-keyboard_arrow_down",
                    "label": "منتجات",
                    "id": "products",
                    "format": "dropdown-list",
                    "description": "",
                    "selected": [],
                    "options": [],
                    "required": true,
                    "multichoice": true,
                    "source": "products",
                    "searchable": true,
                    "maxLength": 8,
                    "minLength": 1
                },
                {
                    "type": "items",
                    "icon": "sicon-link",
                    "label": "رابط عرض الكل",
                    "id": "display_all_url",
                    "value": null,
                    "description": "عند إختيار رابط فارغ سيتم إخفاء زر 'عرض الكل'",
                    "required": false,
                    "format": "variable-list",
                    "searchable": true,
                    "source": "custom",
                    "sources": [
                        {
                            "label": "منتج",
                            "key": "products",
                            "value": "products"
                        },
                        {
                            "label": "تصنيف",
                            "key": "categories",
                            "value": "categories"
                        },
                        {
                            "label": "ماركة تجارية",
                            "key": "brands",
                            "value": "brands"
                        },
                        {
                            "label": "صفحة تعريفية",
                            "key": "pages",
                            "value": "pages"
                        },
                        {
                            "label": "مقالة",
                            "key": "blog_articles",
                            "value": "blog_articles"
                        },
                        {
                            "label": "تصنيف ضمن المدونة",
                            "key": "blog_categories",
                            "value": "blog_categories"
                        },
                        {
                            "label": "التخفيضات",
                            "key": "offers_link",
                            "value": "offers_link"
                        },
                        {
                            "label": "الماركات التجارية",
                            "key": "brands_link",
                            "value": "brands_link"
                        },
                        {
                            "label": "المدونة",
                            "key": "blog_link",
                            "value": "blog_link"
                        },
                        {
                            "label": "رابط خارجي",
                            "key": "custom",
                            "value": "custom"
                        }
                    ]
                }
            ]
        },
        {
            "key": "b89edc4a-ce0b-468f-8323-2da48147bb32",
            "title": "صور مربعة (محسنة)",
            "icon": "sicon-image",
            "path": "home.enhanced-square-banners",
            "fields": [
                {
                    "type": "static",
                    "format": "description",
                    "id": "with-bg",
                    "value": "<div style='padding-top:10px;margin-bottom:30px;border:1px solid #ebebeb;border-radius:5px;text-align:center;overflow:hidden'><h6 style='margin-bottom:10px'>معاينة العنصر</h6><img src='https://cdn.salla.network/images/themes/raed/square-photos.jpg?v=1.1'></div>"
                },
                {
                    "id": "banners",
                    "type": "collection",
                    "format": "collection",
                    "required": true,
                    "minLength": 1,
                    "maxLength": 5,
                    "label": "قائمة الصور",
                    "item_label": "صورة ",
                    "value": [],
                    "fields": [
                        {
                            "type": "string",
                            "icon": "sicon-image",
                            "value": null,
                            "label": "صورة البنر",
                            "id": "banners.image",
                            "format": "image",
                            "required": true,
                            "placeholder": "",
                            "description": "* المقاس المناسب للصورة هو 640×427 بكسل",
                            "settings": {
                                "height": 427,
                                "width": 640
                            }
                        },
                        {
                            "type": "items",
                            "icon": "sicon-link",
                            "label": "الرابط",
                            "id": "banners.url",
                            "value": null,
                            "description": "",
                            "required": false,
                            "format": "variable-list",
                            "searchable": true,
                            "source": "custom",
                            "sources": [
                                {
                                    "label": "منتج",
                                    "key": "products",
                                    "value": "products"
                                },
                                {
                                    "label": "تصنيف",
                                    "key": "categories",
                                    "value": "categories"
                                },
                                {
                                    "label": "ماركة تجارية",
                                    "key": "brands",
                                    "value": "brands"
                                },
                                {
                                    "label": "صفحة تعريفية",
                                    "key": "pages",
                                    "value": "pages"
                                },
                                {
                                    "label": "مقالة",
                                    "key": "blog_articles",
                                    "value": "blog_articles"
                                },
                                {
                                    "label": "تصنيف ضمن المدونة",
                                    "key": "blog_categories",
                                    "value": "blog_categories"
                                },
                                {
                                    "label": "التخفيضات",
                                    "key": "offers_link",
                                    "value": "offers_link"
                                },
                                {
                                    "label": "الماركات التجارية",
                                    "key": "brands_link",
                                    "value": "brands_link"
                                },
                                {
                                    "label": "المدونة",
                                    "key": "blog_link",
                                    "value": "blog_link"
                                },
                                {
                                    "label": "رابط خارجي",
                                    "key": "custom",
                                    "value": "custom"
                                }
                            ]
                        },
                        {
                            "type": "string",
                            "icon": "sicon-format-text-alt",
                            "label": "عنوان رئيسي",
                            "multilanguage": true,
                            "id": "banners.title",
                            "value": null,
                            "required": false,
                            "format": "text",
                            "description": "نص يتم إضافته على الصورة بنمط خط كبير",
                            "placeholder": "أدخل النص هنا...",
                            "hide": false,
                            "minLength": 0,
                            "maxLength": 100
                        },
                        {
                            "type": "string",
                            "icon": "sicon-typography",
                            "label": "نص توضيحي",
                            "multilanguage": true,
                            "id": "banners.description",
                            "value": null,
                            "description": "نص يتم إضافته على الصورة بخط أصغر من العنوان الرئيسي",
                            "format": "textarea",
                            "required": false,
                            "placeholder": "Your text here",
                            "minLength": 0,
                            "maxLength": 255
                        }
                    ]
                }
            ]
        }
    ],
    "support_url": null,
    "description": {
        "ar": "",
        "en": ""
    }
}

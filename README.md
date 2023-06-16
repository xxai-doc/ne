<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

वेबसाइट कोडको अंश खुला स्रोत हो, अनुवादलाई अनुकूलन गर्न मद्दतको लागि स्वागत छ।

## अगाडि-अन्त कोड

* [अगाडि-अन्त कोड](https://github.com/xxai-art/web)
* [सम्पूर्ण साइटको लागि भाषा प्याकहरू](https://github.com/xxai-art/web/tree/main/i18n)
* [लगइन मोड्युलहरूको लागि भाषा प्याकहरू](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [वेबसाइट बहुभाषिक दस्तावेज](https://github.com/xxai-doc)

फ्रन्ट-एन्ड प्रोग्रामिङ भाषा [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) हो, जसले कफीस्क्रिप्ट सिन्ट्याक्समा आधारित केही सुविधाहरू थप्छ, हेर्नुहोस् [./coffee_plus.md](./coffee_plus.md) ।

## वेबसाइट र कागजातहरूको अन्तर्राष्ट्रियकरण

निम्न 3 परियोजनाहरूमा निर्माण गर्नुहोस्

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  `.md` `.mdt` `<+ ./coffee_plus/import.js>`

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  मार्कडाउन अनुवादले कोड र लिङ्कहरू अनुवाद गर्दैन, र अनुवादित वाक्यहरू क्यास गर्नेछ। यदि अनुवाद परिमार्जन गरिएको छ तर मूल पाठ परिमार्जन गरिएको छैन भने, यसलाई पुन: कार्यान्वयन गर्दा अनुवादको परिमार्जन अधिलेखन हुनेछैन।

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` उत्पन्न वेबसाइटहरू अनुवाद गर्न भाषा फाइलहरू।

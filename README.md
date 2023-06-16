<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

यो nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) पहिले स्थापना गर्न सिफारिस गरिन्छ, र त्यसपछि डाइरेक्टरी प्रविष्ट गरेपछि `direnv allow` (डाइरेक्टरी प्रविष्ट गरेपछि [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वचालित रूपमा कार्यान्वयन हुनेछ)।

अर्थ हो: चिनियाँ अनुवाद जापानी, कोरियाली, अंग्रेजी, अन्य सबै भाषाहरूमा अंग्रेजी अनुवाद। यदि तपाइँ केवल चिनियाँ र अंग्रेजीलाई समर्थन गर्न चाहनुहुन्छ भने, तपाइँ केवल `zh: en` लेख्न सक्नुहुन्छ।

अर्थ हो: चिनियाँ अनुवाद जापानी, कोरियाली, अंग्रेजी, अन्य सबै भाषाहरूमा अंग्रेजी अनुवाद। यदि तपाइँ केवल चिनियाँ र अंग्रेजीलाई समर्थन गर्न चाहनुहुन्छ भने, तपाइँ केवल `zh: en` लेख्न सक्नुहुन्छ।

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

### कागजात अनुवाद स्वचालन निर्देशनहरू

कोड रिपोजिटरी [xxai-art/doc](https://github.com/xxai-art/doc) हेर्नुहोस्

यो nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) पहिले स्थापना गर्न सिफारिस गरिन्छ, र त्यसपछि डाइरेक्टरी प्रविष्ट गरेपछि `direnv allow` (डाइरेक्टरी प्रविष्ट गरेपछि [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) स्वचालित रूपमा कार्यान्वयन हुनेछ)।

सयौं भाषाहरूमा अनुवाद गरिएको ठूलो कोड आधारबाट बच्नको लागि, मैले प्रत्येक भाषाको लागि छुट्टै कोड आधार सिर्जना गरें र कोड आधार भण्डारण गर्न संगठन सिर्जना गरें।

वातावरण चर `GITHUB_ACCESS_TOKEN` सेट गर्दै र त्यसपछि [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) चलाउँदा स्वचालित रूपमा कोड भण्डार सिर्जना हुनेछ।

निस्सन्देह, तपाइँ यसलाई कोड आधारमा पनि राख्न सक्नुहुन्छ।

अनुवाद लिपि सन्दर्भ [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

स्क्रिप्ट कोड निम्न रूपमा व्याख्या गरिएको छ:

[bunx](https://bun.sh/docs/cli/bunx) npx को प्रतिस्थापन हो, जुन छिटो छ। अवश्य पनि, यदि तपाइँसँग बन स्थापित छैन भने, तपाइँ यसको सट्टा `npx` प्रयोग गर्न सक्नुहुन्छ।

`bunx mdt zh` ले `.mdt` zh डाइरेक्टरीमा `.md` को रूपमा रेन्डर गर्दछ, तल लिङ्क गरिएका २ फाइलहरू हेर्नुहोस्।

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` अनुवादको लागि कोर कोड हो (यदि तपाइँसँग केवल `nodejs` स्थापना गरिएको छ, तर `bun` र `direnv` स्थापना गरिएको छैन भने, तपाइँ अनुवाद गर्न `npx i18n` पनि चलाउन सक्नुहुन्छ)।

यसले [i18n.yml लाई](https://github.com/xxai-art/doc/blob/main/i18n.yml) पार्स गर्नेछ, यस कागजातमा `i18n.yml` को कन्फिगरेसन निम्नानुसार छ:

```
en:
zh: ja ko en
```

अर्थ हो: चिनियाँ अनुवाद जापानी, कोरियाली, अंग्रेजी, अन्य सबै भाषाहरूमा अंग्रेजी अनुवाद। यदि तपाइँ केवल चिनियाँ र अंग्रेजीलाई समर्थन गर्न चाहनुहुन्छ भने, तपाइँ केवल `zh: en` लेख्न सक्नुहुन्छ।

अन्तिम हो [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , जसले प्रत्येक भाषाको `README.md` को मुख्य शीर्षक र पहिलो उपशीर्षक बीचको सामग्री निकाल्छ `README.md` प्रविष्टि उत्पन्न गर्न। कोड धेरै सरल छ, तपाईं यसलाई आफैलाई हेर्न सक्नुहुन्छ।

Google API नि: शुल्क अनुवादको लागि प्रयोग गरिन्छ। यदि तपाइँ Google पहुँच गर्न सक्नुहुन्न भने, कृपया कन्फिगर गर्नुहोस् र प्रोक्सी सेट गर्नुहोस्, जस्तै:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

अनुवाद स्क्रिप्टले `.i18n` डाइरेक्टरीमा अनुवादित क्यास उत्पन्न गर्नेछ, कृपया यसलाई `git status` साथ जाँच गर्नुहोस् र दोहोर्याइएको अनुवादबाट बच्न कोड भण्डारमा थप्नुहोस्।

कृपया क्यास अद्यावधिक गर्न अनुवाद परिमार्जन गर्दा प्रत्येक पटक `bunx i18n` चलाउनुहोस्।

यदि मूल पाठ र अनुवाद एकै समयमा परिमार्जन गरिएको छ भने, क्यास भ्रमित हुनेछ, त्यसैले यदि तपाइँ परिमार्जन गर्न चाहनुहुन्छ भने, तपाइँ एक मात्र परिमार्जन गर्न सक्नुहुन्छ, र त्यसपछि क्यास अद्यावधिक गर्न `bunx i18n` चलाउनुहोस्।

<div align="center">
	<a href="https://go.warp.dev/PDFMathTranslate" target="_blank">
		<sup>Özel teşekkürler:</sup>
		<br>
		<img alt="Warp sponsorluğu" width="400" src="https://github.com/warpdotdev/brand-assets/blob/main/Github/Sponsor/Warp-Github-LG-02.png">
		<br>
		<h>Warp, birden fazla yapay zeka ajanıyla kodlama için geliştirilmiştir</b>
		<br>
		<sup>macOS, Linux ve Windows için kullanılabilir</sup>
	</a>
</div>

<br>

<div align="center">

English | [简体中文](docs/README_zh-CN.md) | [繁體中文](docs/README_zh-TW.md) | [日本語](docs/README_ja-JP.md) | [한국어](docs/README_ko-KR.md)

<img src="./docs/images/banner.png" width="320px"  alt="PDF2ZH"/>

<h2 id="title">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh/">
    <img src="https://img.shields.io/pypi/v/pdf2zh"></a>
  <a href="https://pepy.tech/projects/pdf2zh">
    <img src="https://static.pepy.tech/badge/pdf2zh"></a>
  <a href="https://hub.docker.com/r/byaidu/pdf2zh">
    <img src="https://img.shields.io/docker/pulls/byaidu/pdf2zh"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Öne Çıkan｜HelloGitHub" /></a>
  <a href="https://gitcode.com/Byaidu/PDFMathTranslate/overview">
    <img src="https://gitcode.com/Byaidu/PDFMathTranslate/star/badge.svg"></a>
  <a href="https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker">
    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Çevrimiçi%20Demo-FF9E0D"></a>
  <a href="https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate">
    <img src="https://img.shields.io/badge/ModelScope-Demo-blue"></a>
  <a href="https://github.com/Byaidu/PDFMathTranslate/pulls">
    <img src="https://img.shields.io/badge/katkılar-bekleniyor-green"></a>
  <a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>
  <!-- Lisans -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/Byaidu/PDFMathTranslate"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

<h2 id="updates">1. Bu ne işe yarar?</h2>

Düzeni koruyarak bilimsel PDF belgelerini çeviren bir araç.

- 📊 Formülleri, grafikleri, içindekiler tablosunu ve açıklamaları korur.
- 🌐 [Birden fazla dili](#kullanım) ve çeşitli [çeviri hizmetlerini](#kullanım) destekler.
- 🤖 [Komut satırı aracı](#kullanım), [etkileşimli kullanıcı arayüzü](#kurulum) ve [Docker](#kurulum) sunar.

<div align="center">
<img src="./docs/images/preview.gif" width="80%"/>
</div>

<h2 id="updates">2. Son Güncellemeler</h2>

- [22 Mart 2026] MiniMax desteği eklendi ([@octo-patch](https://github.com/octo-patch) tarafından PR)
- [22 Mart 2026] OpenAI ile ilgili sorunlar giderildi ([@samqin123](https://github.com/samqin123) tarafından PR)
- [22 Mart 2026] HTTP ile ilgili sorunlar giderildi ([@soukouki](https://github.com/soukouki) tarafından PR)
- [22 Mart 2026] Mac ve ONNX platformlarında daha hızlı model yükleme, GUI başlatma, sürüm yazdırma ve sürekli entegrasyon. ([@reycn](https://github.com/reycn) tarafından)
- [9 Mayıs 2025] pdf2zh 2.0 Önizleme Sürümü [#586](https://github.com/Byaidu/PDFMathTranslate/issues/586): Windows ZIP dosyası ve Docker imajı artık kullanılabilir.

  > [!NOTE]
  >
  > 2.0, organizasyon altındaki yeni bir depoya taşındı: [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next)
  > 
  > 2.0 resmi sürümü yayınlandı.

<h2 id="use-section">3. Kullanım 🌟</h2>
<h3 id="demo">3.1 Çevrimiçi Hizmet 🌟</h3>

Aşağıdaki demolardan birini kullanarak uygulamayı deneyebilirsiniz:

- Kurulum gerektirmeyen [ücretsiz genel hizmet](https://pdf2zh.com/) _(önerilir)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) Ücretsiz kullanım kotası mevcuttur; ayrıntılar için sayfadaki SSS bölümüne bakınız. _(önerilir)_
- [HuggingFace üzerinde barındırılan demo](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- Kurulum gerektirmeyen [ModelScope üzerinde barındırılan demo](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate).

Demolardaki hesaplama kaynakları sınırlıdır, lütfen aşırı kullanımdan kaçının.

<h3 id="install">3.2 Yerel Kurulum</h3>

Farklı kullanım senaryoları için programı kullanmanın çeşitli yöntemlerini sunuyoruz:

<details open>
  <summary>3.2.1 Python: uv ile kurulum</summary>

1. Python kurulu olmalı (3.11 <= sürüm <= 3.12)

2. Paketimizi kurun:

   ```bash
   pip install uv
   uv tool install --python 3.12 pdf2zh
   ```

3. Çeviriyi çalıştırın, dosyalar [mevcut çalışma dizininde](https://chatgpt.com/share/6745ed36-9acc-800e-8a90-59204bd13444) oluşturulur:

   ```bash
   pdf2zh document.pdf
   ```

</details>
<details>
  <summary>3.2.2 Python: pip ile kurulum</summary>

1. Python kurulu olmalı (3.11 <= sürüm <= 3.12)
2. Paketimizi kurun:

   ```bash
   pip install pdf2zh
   ```

3. Çeviriyi çalıştırın, dosyalar [mevcut çalışma dizininde](https://chatgpt.com/share/6745ed36-9acc-800e-8a90-59204bd13444) oluşturulur:

   ```bash
   pdf2zh document.pdf
   ```

</details>
<details>
  <summary>3.3.3 Python: Grafik kullanıcı arayüzü</summary>

1. Python kurulu olmalı (3.11 <= sürüm <= 3.12)

2. Paketimizi kurun:

  ```bash
  pip install pdf2zh
  ```

3. Tarayıcıda kullanmaya başlayın:

   ```bash
   pdf2zh -i
   ```

4. Tarayıcınız otomatik açılmadıysa şu adrese gidin:

   ```bash
   http://localhost:7860/
   ```

   <img src="./docs/images/gui.gif" width="500"/>

Daha fazla ayrıntı için [GUI belgelerine](./docs/README_GUI.md) bakın.

</details>

<details>
  <summary>3.2.4 Uygulama: Windows'ta</summary>

1. [sürüm sayfasından](https://github.com/Byaidu/PDFMathTranslate/releases) pdf2zh-version-win64.zip dosyasını indirin.

2. Sıkıştırmayı açın ve çalıştırmak için `pdf2zh.exe` üzerine çift tıklayın.

  > [!TIP]
  >
  > - Windows kullanıyorsanız ve indirdikten sonra dosyayı açamıyorsanız, lütfen [vc_redist.x64.exe](https://aka.ms/vs/17/release/vc_redist.x64.exe) dosyasını yükleyip tekrar deneyin.
  > 
</details>


<details>

<summary>3.2.5 Referans yöneticisi: Zotero Eklentisi</summary>

Daha fazla ayrıntı için [Zotero PDF2zh](https://github.com/guaguastandup/zotero-pdf2zh) sayfasına bakın.

</details>


<details>
  <summary>3.2.6 Docker: Konteyner ile Dağıtım</summary>

1. İndirin ve çalıştırın:

   ```bash
   docker pull byaidu/pdf2zh
   docker run -d -p 7860:7860 byaidu/pdf2zh
   ```

2. Tarayıcıda açın:

   ```
   http://localhost:7860/
   ```

Bulut hizmetinde docker dağıtımı için:

<div>
<a href="https://www.heroku.com/deploy?template=https://github.com/Byaidu/PDFMathTranslate">
  <img src="https://www.herokucdn.com/deploy/button.svg" alt="Dağıt" height="26"></a>
<a href="https://render.com/deploy">
  <img src="https://render.com/images/deploy-to-render-button.svg" alt="Koyeb'e Dağıt" height="26"></a>
<a href="https://zeabur.com/templates/5FQIGX?referralCode=reycn">
  <img src="https://zeabur.com/button.svg" alt="Zeabur'da Dağıt" height="26"></a>
<a href="https://template.sealos.io/deploy?templateName=pdf2zh">
  <img src="https://sealos.io/Deploy-on-Sealos.svg" alt="Sealos'ta Dağıt" height="26"></a>
<a href="https://app.koyeb.com/deploy?type=git&builder=buildpack&repository=github.com/Byaidu/PDFMathTranslate&branch=main&name=pdf-math-translate">
  <img src="https://www.koyeb.com/static/images/deploy/button.svg" alt="Koyeb'e Dağıt" height="26"></a>
</div>

> [!TIP]
>
> - Docker Hub'a erişemiyorsanız, lütfen [GitHub Container Registry](https://github.com/Byaidu/PDFMathTranslate/pkgs/container/pdfmathtranslate) üzerindeki imajı deneyin.
> ```bash
> docker pull ghcr.io/byaidu/pdfmathtranslate
> docker run -d -p 7860:7860 ghcr.io/byaidu/pdfmathtranslate
> ```
</details>

<details>
  <summary>3.2.* Kurulumda ağ sorunları için çözümler</summary>

  Belirli bölgelerdeki kullanıcılar yapay zeka modelini yüklerken ağ güçlükleriyle karşılaşabilir. Program, yapay zeka modeline (`wybxc/DocLayout-YOLO-DocStructBench-onnx`) bağımlıdır ve bazı kullanıcılar ağ sorunları nedeniyle bunu indiremeyebilir.

  Bu modeli indirme sorununu çözmek için geçici çözüm olarak şu ortam değişkenini kullanın:

  ```shell
  set HF_ENDPOINT=https://hf-mirror.com
  ```

  PowerShell kullanıcıları için:

  ```shell
  $env:HF_ENDPOINT = https://hf-mirror.com
  ```

  Bu çözüm işe yaramazsa veya başka sorunlarla karşılaşırsanız, lütfen [Sık Sorulan Sorular](https://github.com/Byaidu/PDFMathTranslate/wiki#-faq--%E5%B8%B8%E8%A7%81%E9%97%AE%E9%A2%98) sayfasına bakın.

</details>


<h2 id="usage">4. Teknik Detaylar</h2>

### 4.1 Gelişmiş seçenekler

Çeviri komutunu komut satırında çalıştırarak mevcut çalışma dizininde çevrilmiş belge `example-mono.pdf` ve ikidilli belge `example-dual.pdf` oluşturulur. Varsayılan çeviri hizmeti olarak Google kullanılır. Daha fazla desteklenen çeviri hizmetine [BURADAN](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#services) ulaşabilirsiniz.

<img src="./docs/images/cmd.explained.png" width="580px"  alt="cmd"/>

Aşağıdaki tabloda referans için tüm gelişmiş seçenekler listelenmiştir:

| Seçenek               | İşlev                                                                                                         | Örnek                                          |
| --------------------- | ------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- |
| files                 | Yerel dosyalar                                                                                                | `pdf2zh ~/local.pdf`                           |
| links                 | Çevrimiçi dosyalar                                                                                            | `pdf2zh http://arxiv.org/paper.pdf`            |
| `-i`                  | [GUI'ye gir](#gui)                                                                                            | `pdf2zh -i`                                    |
| `-p`                  | [Kısmi belge çevirisi](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#partial)         | `pdf2zh example.pdf -p 1`                      |
| `-li`                 | [Kaynak dil](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#languages)                 | `pdf2zh example.pdf -li en`                    |
| `-lo`                 | [Hedef dil](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#languages)                  | `pdf2zh example.pdf -lo zh`                    |
| `-s`                  | [Çeviri hizmeti](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#services)              | `pdf2zh example.pdf -s deepl`                  |
| `-t`                  | [Çoklu iş parçacığı](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#threads)           | `pdf2zh example.pdf -t 1`                      |
| `-o`                  | Çıktı dizini                                                                                                  | `pdf2zh example.pdf -o output`                 |
| `-f`, `-c`            | [İstisnalar](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#exceptions)                | `pdf2zh example.pdf -f "(MS.*)"`               |
| `-cp`                 | Uyumluluk Modu                                                                                                | `pdf2zh example.pdf --compatible`              |
| `--skip-subset-fonts` | [Font alt kümesini atla](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#font-subset)   | `pdf2zh example.pdf --skip-subset-fonts`       |
| `--ignore-cache`      | [Çeviri önbelleğini yoksay](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#cache)      | `pdf2zh example.pdf --ignore-cache`            |
| `--share`             | Genel bağlantı                                                                                                | `pdf2zh -i --share`                            |
| `--authorized`        | [Yetkilendirme](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#auth)                   | `pdf2zh -i --authorized users.txt [auth.html]` |
| `--prompt`            | [Özel Prompt](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#prompt)                   | `pdf2zh --prompt [prompt.txt]`                 |
| `--onnx`              | [Özel DocLayout-YOLO ONNX modeli kullan]                                                                      | `pdf2zh --onnx [onnx/model/path]`              |
| `--serverport`        | [Özel WebUI portu kullan]                                                                                     | `pdf2zh --serverport 7860`                     |
| `--dir`               | [Toplu çeviri]                                                                                                | `pdf2zh --dir /path/to/translate/`             |
| `--config`            | [Yapılandırma dosyası](https://github.com/Byaidu/PDFMathTranslate/blob/main/docs/ADVANCED.md#cofig)           | `pdf2zh --config /path/to/config/config.json`  |
| `--serverport`        | [Özel gradio sunucu portu]                                                                                    | `pdf2zh --serverport 7860`                     |
| `--babeldoc`          | Çeviri için Deneysel [BabelDOC](https://funstory-ai.github.io/BabelDOC/) arka ucunu kullan                    | `pdf2zh --babeldoc` -s openai example.pdf      |
| `--mcp`               | MCP STDIO modunu etkinleştir                                                                                  | `pdf2zh --mcp`                                 |
| `--sse`               | MCP SSE modunu etkinleştir                                                                                    | `pdf2zh --mcp --sse`                           |

Ayrıntılı açıklamalar için lütfen her seçeneğin tam listesi için [Gelişmiş Kullanım](./docs/ADVANCED.md) belgemize bakın.

<h3 id="downstream">4.2 Alt Düzey Geliştirme</h3>
Alt düzey uygulamalar için lütfen aşağıdakiler hakkında daha fazla bilgi edinmek üzere [API Detayları](./docs/APIS.md) belgemize başvurun:

- [Python API](./docs/APIS.md#api-python), programı diğer Python programlarında nasıl kullanacağınız
- [HTTP API](./docs/APIS.md#api-http), program kurulu bir sunucuyla nasıl iletişim kurulacağı

<h3 id="downstream">4.3 İki ana fork arasındaki farklar</h3>

- [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate): Mevcut ve kararlı sürüm için orijinal proje.

- [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next): Web arayüzü ve ek özellikler içeren bir fork. Bu fork, çok sayıda köşe durumu ele alır, PDF uyumluluğunu iyileştirir ve diğer pek çok çeviri kalitesi geliştirmesinin yanı sıra sütunlar arası ve sayfalar arası anlamsal tutarlılığı, dinamik ölçeklemeyi ve dinamik ölçekleme tutarlılığını optimize eder. Ancak bu fork yalnızca geliştirme amaçlıdır; uyumluluk sorunlarını ele almaz ve topluluk katkılarına yönelik tasarlanmamıştır.

<h2 id="information">5. Proje Bilgileri</h2>
<h3 id="citation">5.1 Alıntı</h3>

Bu çalışma [*2025 Doğal Dil İşlemede Ampirik Yöntemler Konferansı Bildirileri: Sistem Gösterileri*](https://aclanthology.org/2025.emnlp-demos.71/) (EMNLP 2025) tarafından kabul edilmiştir.

Alıntı:

```
@inproceedings{ouyang-etal-2025-pdfmathtranslate,
	    title = "{PDFM}ath{T}ranslate: Scientific Document Translation Preserving Layouts",
	    author = "Ouyang, Rongxin  and
	      Chu, Chang  and
	      Xin, Zhikuang  and
	      Ma, Xiangyao",
	    editor = {Habernal, Ivan  and
	      Schulam, Peter  and
	      Tiedemann, J{\"o}rg},
	    booktitle = "Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing: System Demonstrations",
	    month = nov,
	    year = "2025",
	    address = "Suzhou, China",
	    publisher = "Association for Computational Linguistics",
	    url = "https://aclanthology.org/2025.emnlp-demos.71/",
	    pages = "918--924",
	    ISBN = "979-8-89176-334-0",
	    abstract = "Language barriers in scientific documents hinder the diffusion and development of science and technologies. However, prior efforts in translating such documents largely overlooked the information in layouts. To bridge the gap, we introduce PDFMathTranslate, the world{'}s first open-source software for translating scientific documents while preserving layouts. Leveraging the most recent advances in large language models and precise layout detection, we contribute to the community with key improvements in precision, flexibility, and efficiency. The work is open-sourced at https://github.com/byaidu/pdfmathtranslate with more than 222k downloads."
	}
```

<h3 id="acknowledgement">5.2 Teşekkürler</h3>

- [Immersive Translation](https://immersivetranslate.com), bu projeye aktif katkıda bulunanlara aylık Pro üyelik kullanım kodları sponsorluğu yapmaktadır; ayrıntılar için: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- Yeni arka uç: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Belge birleştirme: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Belge ayrıştırma: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Belge çıkarma: [MinerU](https://github.com/opendatalab/MinerU)

- Belge Önizleme: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Çok iş parçacıklı çeviri: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- Düzen ayrıştırma: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Belge standardı: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Çok dilli Font: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

<h3 id="contrib">5.3 Katkıda Bulunanlar</h3>

<a href="https://github.com/Byaidu/PDFMathTranslate/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/dfa7583da5332a11468d686fbd29b92320a6a869.svg "Repobeats analitik görseli")

Nasıl katkıda bulunacağınıza ilişkin ayrıntılar için lütfen [Katkı Rehberi](https://github.com/Byaidu/PDFMathTranslate/wiki/Contribution-Guide---%E8%B4%A1%E7%8C%AE%E6%8C%87%E5%8D%97)'ne bakın.


<h3 id="star_hist">5.4 Yıldız Geçmişi</h3>

<a href="https://star-history.com/#Byaidu/PDFMathTranslate&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Byaidu/PDFMathTranslate&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Byaidu/PDFMathTranslate&type=Date" />
   <img alt="Yıldız Geçmişi Grafiği" src="https://api.star-history.com/svg?repos=Byaidu/PDFMathTranslate&type=Date"/>
 </picture>
</a>

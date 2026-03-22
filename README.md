div align=center
	a href=httpsgo.warp.devPDFMathTranslate target=_blank
		supÖzel teşekkürlersup
		br
		img alt=Warp sponsorship width=400 src=httpsgithub.comwarpdotdevbrand-assetsblobmainGithubSponsorWarp-Github-LG-02.png
		br
		hWarp, birden fazla yapay zeka ajanıyla kod yazmak için geliştirildib
		br
		supmacOS, Linux ve Windows için kullanılabilirsup
	a
div

br

div align=center

English  [简体中文](docsREADME_zh-CN.md)  [繁體中文](docsREADME_zh-TW.md)  [日本語](docsREADME_ja-JP.md)  [한국어](docsREADME_ko-KR.md)

img src=.docsimagesbanner.png width=320px  alt=PDF2ZH

h2 id=titlePDFMathTranslateh2

p
  a href=httpspypi.orgprojectpdf2zh
    img src=httpsimg.shields.iopypivpdf2zha
  a href=httpspepy.techprojectspdf2zh
    img src=httpsstatic.pepy.techbadgepdf2zha
  a href=httpshub.docker.comrbyaidupdf2zh
    img src=httpsimg.shields.iodockerpullsbyaidupdf2zha
  a href=httpshellogithub.comrepository8ec2cfd3ef744762bf531232fa32bc47 target=_blankimg src=httpsapi.hellogithub.comv1widgetsrecommend.svgrid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small alt=Featured｜HelloGitHub a
  a href=httpsgitcode.comByaiduPDFMathTranslateoverview
    img src=httpsgitcode.comByaiduPDFMathTranslatestarbadge.svga
  a href=httpshuggingface.cospacesreycnPDFMathTranslate-Docker
    img src=httpsimg.shields.iobadge%F0%9F%A4%97-Online%20Demo-FF9E0Da
  a href=httpswww.modelscope.cnstudiosAI-ModelScopePDFMathTranslate
    img src=httpsimg.shields.iobadgeModelScope-Demo-bluea
  a href=httpsgithub.comByaiduPDFMathTranslatepulls
    img src=httpsimg.shields.iobadgecontributions-welcome-greena
  a href=httpst.me+Z9_SgnxmsmA5NzBl
    img src=httpsimg.shields.iobadgeTelegram-2CA5E0style=flat-squeare&logo=telegram&logoColor=whitea
  a href=.LICENSE
    img src=httpsimg.shields.iogithublicenseByaiduPDFMathTranslatea
p

a href=httpstrendshift.iorepositories12424 target=_blankimg src=httpstrendshift.ioapibadgerepositories12424 alt=Byaidu%2FPDFMathTranslate  Trendshift style=width 250px; height 55px; width=250 height=55a

div

h2 id=updates1. Bu ne işe yararh2

Düzeni (layout) koruyarak bilimsel PDF belgesi çevirisi yapar.

- 📊 Formülleri, grafikleri, içindekiler tablosunu ve ek açıklamaları korur.
- 🌐 [Çoklu dil](#usage) desteği ve çeşitli [çeviri hizmetleri](#usage) sunar.
- 🤖 [Komut satırı aracı](#usage), [etkileşimli kullanıcı arayüzü](#install) ve [Docker](#install) sağlar.

div align=center
img src=.docsimagespreview.gif width=80%
div

h2 id=updates2. Son Güncellemelerh2

- [22 Mart 2026] MiniMax desteği eklendi (PR [@octo-patch](httpsgithub.comocto-patch))
- [22 Mart 2026] OpenAI ile ilgili sorunlar düzeltildi (PR [@samqin123](httpsgithub.comsamqin123))
- [22 Mart 2026] HTTP ile ilgili sorunlar düzeltildi (PR [@soukouki](httpsgithub.comsoukouki))
- [22 Mart 2026] Mac ve ONNX platformlarında daha hızlı model yükleme, GUI başlatma, sürüm yazdırma ve sürekli entegrasyon (CI) eklendi. (Yazan [@reycn](httpsgithub.comreycn))
- [9 Mayıs 2025] pdf2zh 2.0 Önizleme Sürümü [#586](httpsgithub.comByaiduPDFMathTranslateissues586) Windows ZIP dosyası ve Docker imajı artık kullanılabilir.

   [!NOTE]
  
   2.0 Sürümü organizasyon altındaki yeni bir depoya taşındı [PDFMathTranslatePDFMathTranslate-next](httpsgithub.comPDFMathTranslatePDFMathTranslate-next)
   
   Sürüm 2.0 resmi yayını yapıldı.

h2 id=use-section3. Kullanım 🌟h2
h3 id=demo3.1 Çevrimiçi Hizmet 🌟h3

Uygulamamızı aşağıdaki demolardan birini kullanarak deneyebilirsiniz

- Kurulum gerektirmeyen [Herkese açık ücretsiz çevrimiçi hizmet](httpspdf2zh.com) _(önerilir)_.
- [Immersive Translate - BabelDOC](httpsapp.immersivetranslate.combabel-doc) Ücretsiz kullanım kotası mevcuttur; ayrıntılar için lütfen sayfadaki SSS bölümüne bakın. _(önerilir)_
- [HuggingFace üzerinde barındırılan demo](httpshuggingface.cospacesreycnPDFMathTranslate-Docker)
- Kurulum gerektirmeyen [ModelScope üzerinde barındırılan demo](httpswww.modelscope.cnstudiosAI-ModelScopePDFMathTranslate).

Demoların işlem kaynaklarının sınırlı olduğunu lütfen unutmayın, bu nedenle lütfen kötüye kullanmaktan kaçının.

h3 id=install3.2 Yerel Kurulumh3

Farklı kullanım senaryoları için, programımızı kullanmanın çeşitli yöntemlerini sunuyoruz

details open
  summary3.2.1 Python uv kullanarak kurulumsummary

1. Python yüklü olmalıdır (3.11 = sürüm = 3.12)

2. Paketimizi kurun

   ```bash
   pip install uv
   uv tool install --python 3.12 pdf2zh
Çeviriyi çalıştırın, dosyalar geçerli çalışma dizininde oluşturulacaktırBashpdf2zh document.pdf
detailsdetailssummary3.2.2 Python pip kullanarak kurulumsummaryPython yüklü olmalıdır (3.11 = sürüm = 3.12)Paketimizi kurunBashpip install pdf2zh
Çeviriyi çalıştırın, dosyalar geçerli çalışma dizininde oluşturulacaktırBashpdf2zh document.pdf
detailsdetailssummary3.3.3 Python Grafik kullanıcı arayüzüsummaryPython yüklü olmalıdır (3.11 = sürüm = 3.12)Paketimizi kurunBashpip install pdf2zh
Tarayıcıda kullanmaya başlayınBashpdf2zh -i
Tarayıcınız otomatik olarak başlamadıysa, şuraya gidinBashhttplocalhost7860
img src=.docsimagesgui.gif width=500Daha fazla detay için GUI belgelerine bakın.detailsdetailssummary3.2.4 Uygulama Windows ÜzerindesummarySürüm release sayfasından pdf2zh-version-win64.zip dosyasını indirin.Zip'ten çıkarın ve çalıştırmak için pdf2zh.exe'ye çift tıklayın.[!TIP]Eğer Windows kullanıyorsanız ve indirdikten sonra dosyayı açamıyorsanız, lütfen vc_redist.x64.exe kurup tekrar deneyin.detailsdetailssummary3.2.5 Referans yöneticisi Zotero EklentisisummaryDaha fazla detay için Zotero PDF2zh sayfasına bakın.detailsdetailssummary3.2.6 Docker Konteynerize Dağıtımsummaryİmajı çekin ve çalıştırınBashdocker pull byaidupdf2zh
docker run -d -p 78607860 byaidupdf2zh
Tarayıcıda açınhttplocalhost7860
Bulut hizmetlerinde docker dağıtımı içindiva href=httpswww.heroku.comdeploytemplate=httpsgithub.comByaiduPDFMathTranslateimg src=httpswww.herokucdn.comdeploybutton.svg alt=Deploy height=26aa href=httpsrender.comdeployimg src=httpsrender.comimagesdeploy-to-render-button.svg alt=Deploy to Koyeb height=26aa href=httpszeabur.comtemplates5FQIGXreferralCode=reycnimg src=httpszeabur.combutton.svg alt=Deploy on Zeabur height=26aa href=httpstemplate.sealos.iodeploytemplateName=pdf2zhimg src=httpssealos.ioDeploy-on-Sealos.svg alt=Deploy on Sealos height=26aa href=httpsapp.koyeb.comdeploytype=git&builder=buildpack&repository=github.comByaiduPDFMathTranslate&branch=main&name=pdf-math-translateimg src=httpswww.koyeb.comstaticimagesdeploybutton.svg alt=Deploy to Koyeb height=26adiv[!TIP]Eğer Docker Hub'a erişemiyorsanız, lütfen GitHub Container Registry üzerindeki imajı deneyin.Bashdocker pull ghcr.iobyaidupdfmathtranslate
docker run -d -p 78607860 ghcr.iobyaidupdfmathtranslate
detailsdetailssummary3.2. Kurulumdaki ağ sorunları için çözümlersummaryBelirli bölgelerdeki kullanıcılar, yapay zeka modelini yüklerken ağ bağlantısı zorluklarıyla karşılaşabilirler. Mevcut program yapay zeka modeline (wybxcDocLayout-YOLO-DocStructBench-onnx) dayanmaktadır ve bazı kullanıcılar bu ağ sorunları nedeniyle modeli indirememektedir.Bu modeli indirmeyle ilgili sorunları gidermek için geçici çözüm olarak aşağıdaki ortam değişkenini kullanınShellset HF_ENDPOINT=[httpshf-mirror.com](httpshf-mirror.com)
PowerShell kullanıcıları içinShell$envHF_ENDPOINT = [httpshf-mirror.com](httpshf-mirror.com)
Bu çözüm işinize yaramazsa veya başka sorunlarla karşılaşırsanız, lütfen Sıkça Sorulan Sorular sayfamıza başvurun.detailsh2 id=usage4. Teknik Detaylarh24.1 Gelişmiş seçeneklerÇevrilmiş belge example-mono.pdf ve iki dilli belge example-dual.pdf'yi geçerli çalışma dizininde oluşturmak için çeviri komutunu komut satırında çalıştırın. Varsayılan çeviri hizmeti olarak Google kullanılır. Desteklenen daha fazla çeviri hizmetini BURADA bulabilirsiniz.img src=.docsimagescmd.explained.png width=580px  alt=cmdAşağıdaki tabloda, referans olması amacıyla tüm gelişmiş seçenekleri listeledikSeçenekİşlevÖrnekfilesYerel dosyalarpdf2zh ~local.pdflinksÇevrimiçi dosyalarpdf2zh httparxiv.orgpaper.pdf-iGUI'ye Girpdf2zh -i-pKısmi belge çevirisipdf2zh example.pdf -p 1-liKaynak dilpdf2zh example.pdf -li en-loHedef dilpdf2zh example.pdf -lo zh-sÇeviri hizmetipdf2zh example.pdf -s deepl-tÇoklu iş parçacığıpdf2zh example.pdf -t 1-oÇıktı dizinipdf2zh example.pdf -o output-f, -cİstisnalarpdf2zh example.pdf -f (MS.)-cpUyumluluk Modupdf2zh example.pdf --compatible--skip-subset-fontsAlt küme fontunu atlapdf2zh example.pdf --skip-subset-fonts--ignore-cacheÇeviri önbelleğini yoksaypdf2zh example.pdf --ignore-cache--shareHerkese açık bağlantıpdf2zh -i --share--authorizedYetkilendirmepdf2zh -i --authorized users.txt [auth.html]--promptÖzel İstem (Prompt)pdf2zh --prompt [prompt.txt]--onnx[Özel DocLayout-YOLO ONNX modeli kullan]pdf2zh --onnx [onnxmodelpath]--serverport[Özel WebUI portu kullan]pdf2zh --serverport 7860--dir[Toplu çeviri]pdf2zh --dir pathtotranslate--configYapılandırma dosyasıpdf2zh --config pathtoconfigconfig.json--serverport[Özel gradio sunucu portu]pdf2zh --serverport 7860--babeldocÇeviri için Deneysel arka uç BabelDOC'u kullanpdf2zh --babeldoc -s openai example.pdf--mcpMCP STDIO modunu etkinleştirpdf2zh --mcp--sseMCP SSE modunu etkinleştirpdf2zh --mcp --sseAyrıntılı açıklamalar ve her seçeneğin tam listesi için lütfen Gelişmiş Kullanım belgemize başvurun.h3 id=downstream4.2 Alt Sistem (Downstream) Geliştirmeh3Alt sistem uygulamaları için, aşağıdakiler hakkında daha fazla bilgi edinmek üzere lütfen API Detayları belgemize başvurunPython API, programın diğer Python programlarında nasıl kullanılacağıHTTP API, programın kurulu olduğu bir sunucu ile nasıl iletişim kurulacağıh3 id=downstream4.3 İki ana çatal (fork) arasındaki farklarh3ByaiduPDFMathTranslate Kararlı sürüm için mevcut ve orijinal proje.PDFMathTranslatePDFMathTranslate-next Web arayüzü (web-ui) ve ek özelliklere sahip bir çatal (fork). Bu çatal çok sayıda uç durumu (marginal cases) ele alır, PDF uyumluluğunu iyileştirir ve sütunlar ile sayfalar arası anlamsal tutarlılığı, dinamik ölçeklendirmeyi ve dinamik ölçeklendirme tutarlılığını optimize etmenin yanı sıra çeviri kalitesinde daha birçok iyileştirme sunar. Ancak bu çatal yalnızca geliştirme amaçlıdır, uyumluluk sorunlarına değinmez ve topluluk katkıları için tasarlanmamıştır.h2 id=information5. Proje Bilgilerih2h3 id=citation5.1 Atıfh3Bu çalışma, 2025 Doğal Dil İşlemede Ampirik Yöntemler Konferansı Bildirileri Sistem Demoları (EMNLP 2025) tarafından kabul edilmiştir.Atıf@inproceedings{ouyang-etal-2025-pdfmathtranslate,
	    title = {PDFM}ath{T}ranslate Scientific Document Translation Preserving Layouts,
	    author = Ouyang, Rongxin  and
	      Chu, Chang  and
	      Xin, Zhikuang  and
	      Ma, Xiangyao,
	    editor = {Habernal, Ivan  and
	      Schulam, Peter  and
	      Tiedemann, J{o}rg},
	    booktitle = Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing System Demonstrations,
	    month = nov,
	    year = 2025,
	    address = Suzhou, China,
	    publisher = Association for Computational Linguistics,
	    url = [httpsaclanthology.org2025.emnlp-demos.71](httpsaclanthology.org2025.emnlp-demos.71),
	    pages = 918--924,
	    ISBN = 979-8-89176-334-0,
	    abstract = Language barriers in scientific documents hinder the diffusion and development of science and technologies. However, prior efforts in translating such documents largely overlooked the information in layouts. To bridge the gap, we introduce PDFMathTranslate, the world{'}s first open-source software for translating scientific documents while preserving layouts. Leveraging the most recent advances in large language models and precise layout detection, we contribute to the community with key improvements in precision, flexibility, and efficiency. The work is open-sourced at [httpsgithub.combyaidupdfmathtranslate](httpsgithub.combyaidupdfmathtranslate) with more than 222k downloads.
	}
h3 id=acknowledgement5.2 Teşekkürlerh3Immersive Translation, bu projeye aktif katkıda bulunanlar için aylık Pro üyelik kullanım kodlarına sponsor olmaktadır, detaylar için bakınız CONTRIBUTOR_REWARD.mdYeni arka uç BabelDOCBelge birleştirme PyMuPDFBelge ayrıştırma Pdfminer.sixBelge çıkarımı MinerUBelge Önizleme Gradio PDFÇok iş parçacıklı çeviri MathTranslateDüzen (Layout) ayrıştırma DocLayout-YOLOBelge standardı PDF Explained, PDF Cheat SheetsÇok dilli Font Go Noto Universalh3 id=contrib5.3 Katkıda Bulunanlarh3a href=httpsgithub.comByaiduPDFMathTranslategraphscontributorsimg src=httpsopencollective.comPDFMathTranslatecontributors.svgwidth=890&button=false aNasıl katkıda bulunabileceğinize dair detaylar için lütfen Katkı Kılavuzuna başvurun.h3 id=star_hist5.4 Yıldız Geçmişih3a href=httpsstar-history.com#ByaiduPDFMathTranslate&Datepicturesource media=(prefers-color-scheme dark) srcset=httpsapi.star-history.comsvgrepos=ByaiduPDFMathTranslate&type=Date&theme=dark source media=(prefers-color-scheme light) srcset=httpsapi.star-history.comsvgrepos=ByaiduPDFMathTranslate&type=Date img alt=Star History Chart src=httpsapi.star-history.comsvgrepos=ByaiduPDFMathTranslate&type=Datepicturea

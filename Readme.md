# Özgeçmiş

Özgeçmişimi içerir.


## Latex Sürümü

Gerekliliklerin kurulumu:
```
sudo apt-get install texlive texlive-latex-extra texlive-luatex texmaker
```

Derleme: Texmaker ile tex dosyaları açılır ve Lualatex ile derlenir.


## Libreoffice Sürümü

Gerekliliklerin kurulumu:
```
sudo apt-get install libreoffice
```

Şablon kaynağı:
https://extensions.libreoffice.org/templates/lebenslauf-im-moderncv-stil-moderncv-style-curriculum-vitae


## Pandoc Sürümü

Kaynak: https://github.com/barraq/pandoc-moderncv.git

Gerekliliklerin kurulumu:
```
sudo apt-get install build-essential ruby ruby-dev pandoc wkhtmltopdf exiftool
sudo gem install compass
sudo gem install susy
```

Derleme:
```
cd pandoc-moderncv/
make html
make pdf HTMLTOPDF=wkhtmltopdf
```

## QR Kodu

Gerekliliklerin kurulumu:
```
sudo apt-get install qrencode
```

Oluşturma:
```
cat huseyinkozan.vcf | qrencode -o "qrcode.png"
```

Pandoc sürümünde kullanma:
```
cp qrcode.png ../pandoc-moderncv/cv/images/
```

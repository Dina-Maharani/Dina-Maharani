<!DOCTYPE html>
<html>
<meta charset='UTF-8' />
<meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport' />
<meta content='IE=edge' http-equiv='X-UA-Compatible' />

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Shippori+Antique:wght@400;500;700&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script><script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script><link rel="stylesheet" href="https://htmlku.com/taubedanya/main/styles.css">

<head>
    <title>S.id/taubedanya - Script HTML buat Kamu</title>
    <meta name="description" content="Feeldream Coding">

<!-- 
  Made with love by feeldream!
  
     Blog: https://feeldream.id
     
  Thanks to all <3
-->
</head>

<body>


    <div id="bodyblur">
        <!-- Wallpaper --><img src="https://i.ibb.co.com/z2dmFv3/f8cb72d992f0d1fb846ef559d58ededc.jpg" id="wallpaper" />
        <div id="beneranblur"></div>
    </div>

    <div id="bodyblur">
        <!-- Wallpaper --><img src="https://i.ibb.co.com/z2dmFv3/f8cb72d992f0d1fb846ef559d58ededc.jpg" id="wallpaper" />
        <div id="beneranblur"></div>
    </div>

    <div id='Content'>

        <!-- Tombol LOVE -->
        <div id="loveIn">
            <a href="#" class="lovein">&#10084;</a>
        </div>
        <p id="ket">Sentuh LOVEnya!</p>

        <div class="kumpulanstiker">
            <!-- Stiker untuk Konten -->
            <img src="https://feeldreams.github.io/pandapanah.gif" id="fotostiker" />
            <img src="https://feeldreams.github.io/pusn.gif" id="fotostiker1" />
            <img src="https://feeldreams.github.io/mikir.gif" id="fotostiker2" />
            <img src="https://feeldreams.github.io/g5.gif" id="fotostiker3" />
            <img src="https://feeldreams.github.io/mmm.gif" id="fotostiker4" />
            <img src="https://feeldreams.github.io/emawh.gif" id="fotostiker5" />
        </div>

        <p id="halo" class="halo"></p>

        <div>
            <blockquote id='bq' data-text=''>

                <p id="kalimat"><span style="font-size:15px">Aku Punya Pesan<br>Nih buat Kamu 🫢❤️</span></p>
                <p id="kalimatb"></p>

                <!-- Pesan -->
                <p id="pesan1"><b style="font-size:16px">Klik 4 LOVE ini! 🫣</b></p>
                <div id="kolombaru">
                    <li id="lv1">💗</li>
                    <li id="lv2">💗</li>
                    <li id="lv3">💗</li>
                    <li id="lv4">💗</li>
                </div>

                <p id="pesan2"></p>
                <p id="pesan3"></p>
                <p id="pesan4" class="sty2b"><b>Kamu kayaknya harus bayar denda ke aku deh faaa </b></p>
                <p id="pesan5" class="sty2b">iyaa bener<br>bayar denda </p>
                <p id="pesan6" class="sty2b">mau tau kenapaa? </p>
                <p id="pesan7" class="sty2b left"><b>cuz you spend so much time in my mind......<br>hehe! 👉👈</b></p>
                <p id="pesan8" class="sty2b left"><i>Hehehe</i> <br>sayaangg acaaaa nakall lagii yaa tadii maaf yaaa sayangg tadii acaaa nggaa seharusnya ngucapin kata tadii, maafin sikapku tadiii yaaa faaa yangg ngebuatt kamuu kecewa sama sakittt hatii,acaaa salahh ngetikk kayakk tadii ituuu konyoll faaa, dann akuu bnerr benrrr nyesel, akuu tauuu kamuu mestii sakitt hati banget sekarang, akuu gapapa kalo nggga kamu maafin, akuu gamauu ngulang lagi, aku gamauuu lost kontak, akuuu sayaangg kamuu faa, loveee youu sayaangg</p>

                <!-- Tombol Lanjut -->
                <p id="opsL">Klik untuk Lanjut</p>
            </blockquote>
        </div>

        <!-- Tombol Kirim Pesan -->
        <div id="Tombol"><a id="By">&#128140; Balas</a></div>

        <!-- Pesan Ditolak -->
        <div id="pesanditolak">
            <img id="stikerditolak" src="https://feeldreams.github.io/weee.gif" />
            <p id="kataditolak">yaudaaa gapapaa sayangg mungkin kamu masih nggaa mood</p>
        </div>

    </div>

    <script>
        function welcome() {
            teksWelcome = "Hai, " + nama + " ✨";
        }

        //Variable Pertanyaan Akhir
        var tanya = 'maafinn acaaa yaaa';
        var opstanya = 'haruss maafin';
        var tompositif = 'iyaaaa';
        var tomnegatif = 'Engga';

        async function pertanyaan() {
            var { isConfirmed: prtanya } = await swals.fire({ title: nama + ' ' + tanya, text: '' + opstanya, imageUrl: '' + fotostiker5.src, showCancelButton: true, confirmButtonText: '' + tompositif, cancelButtonText: '' + tomnegatif, });
            if (prtanya) {
                pesanwhatsapp = "Iyaa " + nama + " iyaaa sayaang aku maafin kok! ><";
                menujuWA();
            } else {
                pesanwhatsapp = nama + " engga kangen kamu wleee! :p";
                await swalst.fire({ title: '' + kataditolak.innerHTML, timer: 2000, imageUrl: '' + stikerditolak.src, });
                menujuWA();
            }
        }
    </script>
    <script src="https://htmlku.com/taubedanya/main/script.js"></script>

</body>
</html>

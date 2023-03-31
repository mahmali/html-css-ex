<script setup>

</script>

<template>
    <div class="container">
        <form action="https://httpbin.org/post" method="post">
            <div class="form-row">
                <label for="adi">Adı:</label>
                <!-- value değeri içinde yazılı olarak gelir sıfırlansa bile orda kalır -->
                <input name="adi" type="adi" value="" required placeholder="Adınız Soyadınız">
            </div>
            <div class="form-row">
                <label for="number">Numara:  </label>
                <input name="telefon numarasi" type="tel" required>
                <!-- required dolsurulması zorunlu alan olarak tanımlar -->
            </div>
            <div class="form-row">
                <label for="email">Email:  </label>
                <input name="email" type="email">
            </div>
            <div class="form-row">
                <label for="mesaj">Mesaj:  </label>
                <textarea name="mesaj" id="mesaj" cols="20" rows="10"></textarea>
            </div>
            <div class="form-row">
                <label for="sehir">Şehir</label>
                <select name="sehir" id="sehir">
                    <option value="Elazığ">Elazığ</option>
                    <option value="Isparta" selected>Isparta</option>
                    <!-- selected yazılan optionun seçili olarak gelmesini sağlar -->
                </select>
            </div>
            <div class="form-row">
                <label for="">Sevdiğiniz Renk</label>
                    <div class="radio-container">
                        <label for="Kırmızı"> <input type="radio" name="renk" id="Kırmızı" value="kırmızı">Kırmızı</label>
                        <label for="Mavi"> <input type="radio" name="renk" id="Mavi" value="mavi">Mavi</label>
                        <label for="Yeşil"> <input type="radio" name="renk" id="Yeşil" value="yeşil">Yeşil</label>
                    </div>
                <!-- checked radio butonun default olarak seçili olarak gelmesini sağlar -->
                <!-- //name verilirse sadece bir tane radio buton seçilir -->
            </div>
            <div class="form-row">
                <button type="reset">Sıfırla</button>
                <button style="margin-left: 14px;" type="submit">Gönder</button>

            </div>
        </form>
    </div>
</template>

<style scoped>
.container{
    font-family: Arial, Helvetica, sans-serif; /*İşletim sisteminde sırayla hangi font varso onu kullan*/
    font-size: 20px;
}
select,
input[type=adi],
input[type=tel],
input[type=email],
button,
textarea {
    width: 100%;
    border-radius: 5px;
    height: 45px;
    border: 1px solid rgba(0, 0, 0, 0.2);
    padding-left: 15px;
    padding-right: 15px; /* input içindeki padding degeridir.*/
    font-size: inherit; /* inherit kapsayıcısını font size özelliği ne ise içeriğininde o özelliği almasına yarar*/
    font-family: inherit;
}
input[type=adi]:focus, /* focus inputa tıklayıp yazı yazarkenki verilen css özellikleridir*/
input[type=tel]:focus,
input[type=email]:focus,
textarea:focus {
    border-color: cornflowerblue;
}
input[type=adi]::placeholder{
    color: rgba(0, 0, 0, 0.2);
}
form{
    margin-left: auto;
    margin-right: auto;
    width: 600px;
    padding: 50px;
}
.form-row{
    margin-bottom: 20px;

}
.form-row label{
    margin-bottom: 6px;
}
textarea{
    height: 100px;
    padding: 15px;
    min-height: 50px;
    max-height: 200px;
}
.radio-container label{
    margin-left: 20px;
}
.radio-container label input{
    margin-right: 10px;
}
button{
    width: auto;
    border: 0;
}
button[type="su"]

</style>

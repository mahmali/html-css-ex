<script setup>

</script>

<template>
    <div class="container">
        <form action="https://httpbin.org/post" method="post">
            <div>
                <label for="adi">Adİ:</label>
                <!-- value değeri içinde yazılı olarak gelir sıfırlansa bile orda kalır -->
                <input name="adi" type="adi" value="Adi Soyadi" required>
            </div>
            <div>
                <label for="number">Numara:  </label>
                <input name="telefon numarasi" type="tel" required>
                <!-- required dolsurulması zorunlu alan olarak tanımlar -->
            </div>
            <div>
                <label for="email">Email:  </label>
                <input name="email" type="email">
            </div>
            <div>
                <label for="mesaj">Mesaj:  </label>
                <textarea name="mesaj" id="mesaj" cols="20" rows="10"></textarea>
            </div>
            <div>
                <label for="sehir">Şehir</label>
                <select name="sehir" id="sehir">
                    <option value="Elazığ">Elazığ</option>
                    <option value="Isparta" selected>Isparta</option>
                    <!-- selected yazılan optionun seçili olarak gelmesini sağlar -->
                </select>
            </div>
            <div>
                <label for="">Sevdiğiniz Renk</label>

                <input type="radio" name="renk" id="Kırmızı" value="kırmızı"> <label style="display: inline;" for="Kırmızı">Kırmızı</label>
                <input type="radio" name="renk" checked value="Turuncu">Turuncu 
                <!-- checked radio butonun default olarak seçili olarak gelmesini sağlar -->
                <!-- //name verilirse sadece bir tane radio buton seçilir -->
            </div>
            <div class="buttons">
                <button type="reset">Sıfırla</button>
                <button style="margin-left: 14px;" type="submit,">Gönder</button>

            </div>
        </form>
    </div>
</template>

<style scoped>
label {
    display: block;
    margin-top: 15px;
}
select,
input[type=adi],
input[type=tel],
input[type=email],
textarea {
    width: 300px;
}
.buttons {
    padding: 15px;
}

</style>

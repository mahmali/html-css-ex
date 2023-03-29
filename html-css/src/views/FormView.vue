<script setup>

</script>

<template>
    <div class="container">
        <form action="">
            <div>
                <label for="adi">Adı:  </label>
                <input type="adi">
            </div>
            <div>
                <label for="number">Numara:  </label>
                <input type="tel">
            </div>
            <div>
                <label for="email">Email:  </label>
                <input type="email">
            </div>
            <div>
                <label for="mesaj">Mesaj:  </label>
                <textarea id="mesaj" cols="20" rows="10"></textarea>
            </div>
            <div>
                <label for="sehir">Şehir</label>
                <select name="sehir" id="">
                    <option value="">Elazığ</option>
                    <option value="">Isparta</option>
                </select>
            </div>
        </form>
    </div>
</template>

<style scoped>
label {
    display: block;
}
select, input, textarea {
    width: 300px;
}

</style>

<template>
    <div>
        <h1>Hallo Dunia</h1>
        <p>Ini Komponen Gue</p>
        <!--props-->
        <h2>Nama : {{ nama }}</h2>
        <br>
        <h3>Umur : {{ umur }}</h3>
        <br>
        <h3>Jenis Kelamin : {{ jk }}</h3>
        <br>
        <h3>Alamat : {{ alamat }}</h3>
    </div>
</template>

<script>
export default {
    props:['nama', 'umur', 'jk', 'alamat'],

}
</script>

<style>
h1{
    color: red;
}

p{
    size: 16px;
}
</style>
<script setup>

</script>

<template>
    <section>
        <div class="contact-form">
            <form>
                <h1>Get in touch</h1>
                <input type="text" id="firstName" placeholder="First Name" required />
                <input type="text" id="lastName" placeholder="Last Name" required />
                <input type="email" id="email" placeholder="Email" required />
                <input type="text" id="mobile" placeholder="Mobile" required />
                <h4>Type Your Message Here...</h4>
                <textarea required></textarea>
                <input type="submit"  id="button" />
            </form>
            <img src="\src\assets\email.jpg" class="img">
        </div>
    </section>
</template>

<style scoped>

.contact-form {
    min-height: 100vh;
    display: flex;
    gap: 8rem;
    justify-content: center;
    align-items: center;
}


.contact-form form {
    width: 670px;
    height: 600px;
    display: flex;
    justify-content: center;
    border-radius: 15px;
    background: #f0eada;
    /* backdrop-filter: blur(30px); */
    flex-wrap: wrap;
}
.contact-form h1{
    color: #006A71;
}

.contact-form form h1 {
    font-weight: 700;
    line-height: 1;
    margin-top: 20px;
    width: 500px;
    text-align: center;
    font-size: 3rem;
}


.contact-form form input {
    width: 300px;
    height: 50px;
    padding-left: 10px;
    outline: none;
    border: none;
    font-size: 20px;
    margin-bottom: 10px;
    background: none;
    border-bottom: 2px solid black;
    color: black;
}

.contact-form form input::placeholder {
    color: black;
}

.contact-form form #lastName,
.contact-form form #mobile {
    margin-left: 20px;
}

.contact-form form h4 {
    color: black;
    font-weight: 300;
    width: 600px;
    margin-top: 20px;
}

.contact-form form textarea {
    background: none;
    border: none;
    border-bottom: 2px solid black;
    color: black;
    font-weight: 200;
    font-size: 20px;
    padding: 10px;
    outline: none;
    min-height: 90px;
    max-height: 90px;
    min-width: 620px;
    max-width: 620px;
}

.contact-form form h4 {
    font-size: 20px;
}

.contact-form form #button {
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: #f0eada;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: black;
    letter-spacing: 0.2rem;
    font-weight: 600;
    border: 2px solid black;
    transition: 0.3s ease;
    cursor: pointer;
}

.contact-form form #button:hover {
    transform: scale3d(1.03);
    background-color: #006A71;
    color: white;
    box-shadow: 0 0 25px #006A71;
}

.img {
    position: relative;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px solid #006A71;
    cursor: pointer;
    transition: 0.2s linear;
}
</style>
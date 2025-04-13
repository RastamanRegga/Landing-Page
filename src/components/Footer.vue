<template>
    <footer class="footer" id="footer">
        <div class="footer-content">
            <p>&copy; 2025 Regga. All rights reserved.</p>
            <div class="icons">
                <a style="--accent-color: black" href="https://github.com/RastamanRegga"><i class="fa-brands fa-github"></i></a>
                <a style="--accent-color: #365ee0" href="https://www.linkedin.com/in/rastaman-regga-pratama-001882321"><i class="fa-brands fa-linkedin"></i></a>
                <a style="--accent-color: #e32262" href="https://www.instagram.com/ "><i class="fa-brands fa-instagram"></i></a>
                <a style="--accent-color: #00c939" href="https://wa.me/6285179586256"><i class="fa-brands fa-whatsapp"></i></a>
            </div>
        </div>
    </footer>
</template>

<style scoped>
.footer {
    background-color: #222;
    color: #fff;
    padding: 20px;
    text-align: center;
}

.footer-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

.icons a {
    margin: 0 10px;
    color: white;
    font-size: 2rem;
    transition: color 0.3s;
}

.icons a:hover {
    color: var(--accent-color);
}
</style>

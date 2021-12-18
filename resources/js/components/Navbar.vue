<template>
    <nav class="main-nav">
        <ul>
            <li>
                <router-link to="/" class="router-link"> Home </router-link>
            </li>
            <li>
                <router-link to="/user/account" class="router-link">
                    Profile
                </router-link>
            </li>
            <li>
                <router-link to="/user/account" class="router-link">
                    Dummy A
                </router-link>
            </li>
            <li>
                <router-link to="/user/account" class="router-link">
                    Dummy B
                </router-link>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: "Navbar",
};
</script>

<style scoped>
.main-nav {
    padding: 1.5rem;
}

.main-nav ul {
    display: grid;
    grid-gap: 20px;
    padding: 0;
    list-style: none;
    grid-template-columns: repeat(4, 1fr);
}

.main-nav .router-link {
    background: var(--primary);
    display: block;
    text-decoration: none;
    padding: 0.8rem;
    text-align: center;
    color: var(--dark);
    text-transform: uppercase;
    font-size: 1.1rem;
    box-shadow: var(--shadow);
}

.main-nav .router-link:hover {
    background: var(--dark);
    color: var(--light);
}

/* Media Queries */
@media (max-width: 700px) {
    .main-nav ul {
        grid-template-columns: 1fr;
    }
}
</style>

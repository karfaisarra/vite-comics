<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            menuEl: [
                {
                    name: 'CHARACTERS',
                    href: '#'
                },
                {
                    name: 'COMICS',
                    href: '#'
                },
                {
                    name: 'MOVIES',
                    href: '#'
                },
                {
                    name: 'TV',
                    href: '#'
                },
                {
                    name: 'GAMES',
                    href: '#'
                },
                {
                    name: 'COLLECTIBLES',
                    href: '#'
                },
                {
                    name: 'VIDEOS',
                    href: '#'
                },
                {
                    name: 'FANS',
                    href: '#'
                },
                {
                    name: 'NEWS',
                    href: '#'
                },
                {
                    name: 'SHOP',
                    href: '#'
                },
            ]
        }
    }
}
</script>
<template>
    <header id="site_header">
        <div class="container">
            <div class="navbar">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <div class="menu">
                    <ul>
                        <li v-for="el in menuEl">
                            <a :class="el.name === 'COMICS' ? 'active' : ''" :href="el.href"> {{ el.name }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
.navbar {

    display: flex;
    align-items: center;
    padding: 0.5rem 0;
    justify-content: space-around;

    img {
        width: 80px;
    }

    .menu ul {
        list-style: none;
        display: flex;

        li {
            padding: 0 1rem;

            a:not(.active) {
                text-decoration: none;
                color: black;
                padding-bottom: 2.7rem;
                font-weight: bold;

                &:hover {
                    color: #0282F9;
                    border-bottom: 4px solid #0282F9;
                }
            }
        }
    }
}

.active {
    color: #0282F9;
    border-bottom: 4px solid #0282F9;
    padding-bottom: 2.7rem;
    text-decoration: none;
    font-weight: bold;
}
</style>
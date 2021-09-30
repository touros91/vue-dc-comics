<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="../assets/images/dc-logo.png" alt="Logo DC">
            </div>
            <div class="menu">
                <ul>
                    <li v-for="(item, index) in menu" :key="index">
                        <a :href="item.href" :class="{active : item.status}">{{item.name}}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data (){
        return {
            menu: [
                {
                    name: 'CHARACTERS',
                    href: '#',
                    status: false
                },
                {
                    name: 'COMICS',
                    href: '#',
                    status: true
                },
                {
                    name: 'MOVIES',
                    href: '#',
                    status: false
                },
                {
                    name: 'TV',
                    href: '#',
                    status: false
                },
                {
                    name: 'GAMES',
                    href: '#',
                    status: false
                },
                {
                    name: 'COLLECTBLES',
                    href: '#',
                    status: false
                },
                {
                    name: 'VIDEOS',
                    href: '#',
                    status: false
                },
                {
                    name: 'FANS',
                    href: '#',
                    status: false
                },
                {
                    name: 'NEWS',
                    href: '#',
                    status: false
                },
                {
                    name: 'SHOP',
                    href: '#',
                    status: false
                }       
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/Variables.scss';
    header {
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
            .logo {
                max-width: 70px;
                img {
                    width: 100%;
                }
            }
            .menu {
                ul {
                    list-style: none;
                    display: flex;
                    li {
                        padding: 10px;
                        a {
                            text-decoration: none;
                            color: #57535B;
                            font-weight: bold;
                            font-size: 15px;
                            &.active {
                                color: $mainColor;
                                border-bottom: 5px solid $mainColor;
                                padding-bottom: 100%;
                            }
                        }
                    }
                }
            }
        }
    }
</style>
<template>
    <header>
        <div class="container">

            <div class="logo">
                <img src="@/assets/images/dc-logo.png" alt="">
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
                            padding-bottom: 100%;
                            &.active {
                                color: #1D8BFA;
                                border-bottom: 4px solid #1D8BFA;
                            }
                        }
                    }
                }
            }
        }
    }
</style>
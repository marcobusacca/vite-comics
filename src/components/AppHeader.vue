<!-- SCRIPT VUE.JS -->
<script>
export default {
    data() {
        return {
            // MENU ITEM LINK OBJECT ARRAY
            menuItem: [
                {
                    label: 'CHARACTERS',
                    link: '#',
                    active: false,
                },
                {
                    label: 'COMICS',
                    link: '#',
                    active: false,
                },
                {
                    label: 'MOVIES',
                    link: '#',
                    active: false,
                },
                {
                    label: 'TV',
                    link: '#',
                    active: false,
                },
                {
                    label: 'GAMES',
                    link: '#',
                    active: false,
                },
                {
                    label: 'COLLECTIBLES',
                    link: '#',
                    active: false,
                },
                {
                    label: 'VIDEOS',
                    link: '#',
                    active: false,
                },
                {
                    label: 'FANS',
                    link: '#',
                    active: false,
                },
                {
                    label: 'NEWS',
                    link: '#',
                    active: false,
                },
                {
                    label: 'SHOP',
                    link: '#',
                    active: false,
                },
            ]
        }
    },
    methods: {
        // FUNZIONE CHE ATTIVA L'ELEMENTO DEL MENU QUANDO L'UTENTE VA IN HOVER CON IL CURSORE DEL MOUSE
        activeMenuItem(index) {
            this.menuItem[index].active = true;
        },

        // FUNZIONE CHE DISATTIVA L'ELEMENTO DEL MENU QUANDO L'UTENTE TOGLIE IL CURSORE DEL MOUSE
        inActiveMenuItem(index) {
            this.menuItem[index].active = false;
        }
    }
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <header>
        <!-- Header Container -->
        <div class="container">
            <!-- Header Row -->
            <div class="row">
                <!-- Header Logo Col -->
                <div class="col">
                    <!-- Header Logo -->
                    <img src="../assets/dc-logo.png" alt="">
                </div>
                <!-- Header Menu Col -->
                <div class="col">
                    <!-- Header Menu -->
                    <ul>
                        <li v-for="(item, index) in menuItem" :key="index" :class=" item.active ? 'active' : '' " @mouseover="activeMenuItem(index)" @mouseleave="inActiveMenuItem(index)">
                            <a :href="item.link" v-text="item.label"></a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

header {
    height: 120px;

    .container {
        max-width: 1600px;
        margin: 0 auto;
        height: 100%;

        .row {
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: space-between;

            .col {
                height: 100%;
                display: flex;
                align-items: center;

                img {
                    width: 80%;
                    cursor: pointer;
                }

                ul {
                    height: 100%;
                    display: flex;
                    align-items: center;
                }

                li {
                    display: flex;
                    align-items: center;
                    height: 100%;
                    font-size: 14px;
                    font-weight: 700;
                    padding: 15px;
                    border-bottom: 5px solid transparent;
                    cursor: pointer;
                }

                .active {
                    color: #0282F9;
                    border-bottom-color: #0282F9;
                }
            }
        }
    }
}
</style>
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
                    <img src="../assets/dc-logo.png" alt="dc-header-logo">
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
// IMPORTO IL FILE _VARIABLES.SCSS
@use '../styles/partials/variables' as *;

header {
    height: 120px;

    .row {
        justify-content: space-between;

        .col {
            display: flex;
            align-items: center;
            height: 100%;

            img {
                width: 80%;
                cursor: pointer;
            }

            ul {
                display: flex;
                align-items: center;
                height: 100%;
            }

            li {
                display: flex;
                align-items: center;
                height: 100%;
                padding: 15px;
                font-size: 14px;
                font-weight: 700;
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
</style>
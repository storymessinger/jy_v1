<template>
  <div class="main">
    <div class="name">
        Jiyoun
    </div>
    <masonry :cols="{default: 4, 1000: 3, 700: 2, 400: 2}" :gutter="{default: 40}">
        <div v-for="(item, index) in items" :key="index">
            <div class="project">
                <router-link :to="item.detail" class="project__img">
                    <img :src='item.img' >
                </router-link>
                <div class="project__name">
                    <span>{{item.name}}</span>
                    <span>{{item.type}}</span>
                </div>
                <div class="project__info">
                    <p>Client / {{item.client}}</p>
                    <p>location / {{item.location}}</p>
                    <p>Design Period / {{item.design_period}}</p>
                </div>
            </div>
        </div>
    </masonry>

    <router-view></router-view>

  </div>
</template>

<script>

export default {

    components: {
        // appFooter: Footer
    },

    data: function() {
        return {
            items: [
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                },
                { 
                    name: 'SOMETHING FUN',
                    type: 'play',
                    client: 'myself',
                    location: 'Daejeon, Korea',
                    design_period: '2017.01 - 2017.08',
                    img: "https://via.placeholder.com/300x300",
                    detail: "/projects"
                }
            ]
        }
    }
}

</script>

<style lang="scss">

    .main {
        margin: 100px 2% 0 2%;
    }
    .name {
        margin-bottom: 40px;
        display: flex;
        width: 40%;
        justify-content: space-between;
        font-family: 'Noto Sans KR';
        font-weight: 300;
        font-size: 14px;
        .filter__menu {
            color: #919192;
        }
        .select {
            color: black;
        }
    }

    .project {

        border-bottom: solid 1px rgba(0,0,0,0.4);
        margin-bottom: 40px;


        .project__img {
            width: 100%;
            img {
                 width: 100%;
                 margin-bottom: 40px;
            }
            margin-bottom: 40px;
        }
        .project__name {
            display: flex;
            justify-content: space-between;
            font-family: 'Noto Sans KR';
            font-weight: 600;
            font-size: 12px;
            margin-bottom: 25px;
        }
        .project__info {
            font-family: 'Noto Sans KR';
            font-weight: 200;
            font-size: 12px;
            p {
                margin: 0;
            }
            margin-bottom: 40px;
        }
    }
    
    
</style>


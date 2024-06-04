<template>
    <div class="header">
        <AppContainer>
            <div class="navbar__">
                <NuxtLink to="/">
                    <div class="navbar__logo">
                        <svg width="10" height="37" viewBox="0 0 10 37" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M4.10388 18.2052C4.10388 12.0097 5.28016 6.8309 8.83512 1.27087C8.96582 1.08024 9.75 0 9.75 0C9.75 0 7.50201 1.04846 5.69839 2.95476C4.41756 4.28917 3.29357 5.78244 2.32641 7.8476C0.496647 11.7555 0 14.9327 0 18.2052C0 21.4776 0.496647 24.6548 2.32641 28.5627C3.29357 30.6279 4.41756 32.1211 5.69839 33.4555C7.52815 35.3618 9.75 36.4103 9.75 36.4103C9.75 36.4103 8.96582 35.3301 8.83512 35.1394C5.28016 29.5794 4.10388 24.4006 4.10388 18.2052Z" fill="url(#paint0_linear_391_756)"/>
                         <defs>
                        <linearGradient id="paint0_linear_391_756" x1="4.875" y1="0" x2="4.875" y2="36.4103" gradientUnits="userSpaceOnUse">
                        <stop stop-color="#F9F9F9"/>
                        <stop offset="1" stop-color="#8F8F8F"/>
                        </linearGradient>
                        </defs>
                        </svg>
                    </div>
                </NuxtLink>
                <div class="navbar__buttons">
                    <div class="navbar__products">
                        <NuxtLink to="/products">продукты</NuxtLink>
                        <svg width="10" height="6" viewBox="0 0 10 6" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M5.2733 5.08875L9.2558 0.909003C9.32229 0.839262 9.35938 0.746606 9.35938 0.650253C9.35938 0.5539 9.32229 0.461245 9.2558 0.391503L9.2513 0.387003C9.21907 0.353076 9.18028 0.326062 9.13728 0.307601C9.09428 0.289141 9.04797 0.279622 9.00118 0.279622C8.95438 0.279622 8.90808 0.289141 8.86508 0.307601C8.82208 0.326062 8.78328 0.353076 8.75105 0.387003L5.00105 4.323L1.25255 0.387002C1.22032 0.353076 1.18153 0.326061 1.13853 0.307601C1.09553 0.28914 1.04922 0.279621 1.00243 0.279621C0.955635 0.279621 0.909329 0.28914 0.86633 0.307601C0.823329 0.326061 0.784535 0.353076 0.752304 0.387002L0.747804 0.391503C0.681321 0.461244 0.644232 0.553899 0.644232 0.650252C0.644232 0.746605 0.681321 0.839261 0.747804 0.909002L4.7303 5.08875C4.76533 5.12551 4.80745 5.15478 4.85412 5.17477C4.90079 5.19477 4.95103 5.20508 5.0018 5.20508C5.05258 5.20508 5.10282 5.19477 5.14949 5.17477C5.19616 5.15478 5.23828 5.12551 5.2733 5.08875Z" fill="white"/>
                        </svg>
                    </div>
                    <div class="navbar__buttons-drivers">
                        <NuxtLink to="/drivers">драйвера</NuxtLink>
                    </div>
                </div>
                    <div class="navbar__buttons-support">
                        <NuxtLink to="/support">поддержка</NuxtLink>
                    </div>
            </div>
        </AppContainer>
    </div>
    
</template>


<style scoped lang="scss">



.header {
    width: 100%;
    height: 100px;
    background: linear-gradient(to bottom, #0e0e0e, transparent 78%);
    position: fixed;
    top: 0px;
    z-index: 10;
    
}

.navbar__ {
    display: flex;
    width: 1200px;
    margin-top: 20px;
    align-items: center;
    justify-content: space-between;
    color: #FFFFFF;
    position: fixed;
    top: 0px;
    text-align: center;

    &logo {
        padding-right: 25px;
    }

    &products {
        & svg {
            margin-left: 5px;
            margin-top: 2px;
        }
    }

    &buttons {
        display: flex;
        &-drivers {
            margin-left: 40px;
            margin-right: -40px;
        }
        &-support {
            // margin-left: 20px;
        }
    }
}
a {
    text-decoration: none;
    color: #FFFFFF;
    padding-top: 10px;
    margin-top: -10px;
    transition: .15s;
    font-size: 14px;
    font-weight: 400;
    & svg {
        transition: .15s;
    }
    &:hover {
        color: grey;
        transition: .15s;
    }
    &:hover svg {
        filter: brightness(125%);
        transition: .15s;
    }
}
.navbar__products {
    &:hover a{
        color: grey;
        transition: .15s;
    }
    &:hover svg path {
            fill: grey;
            transition: .15s;
        }
        & svg path {
            fill: white;
            transition: .15s;
        }
        &:hover svg {
            transform: rotate(90deg);
            transition: .15s;
        }
        & svg {
            transition: .15s;
        }
}







</style>


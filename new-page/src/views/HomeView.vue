<template>
    <div>
        <div class="home h-100" style="min-height: 100vh;width: 100vw;">
            <div v-if='this.showSideBar'>
                <sidebar @closeSidebarEvent="closeSidebar"  SideBar='sidebar'></sidebar>
            </div>
            <div class="container  " style="padding:0px 20px 0px 20px">
                <div class="wrapper ">
                    <div class="header" style="padding-top: 10px;">
                        <div v-if="this.$isMobile()">
                            <div class="row">
                                <div class="col-auto text-start">
                                    <div class="img">
                                        <img style="height:8vh;width: 10vw;" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/logo-new@2x.png">
                                    </div>
                                </div>
                                <div class="col text-end">
                                    <svg t="1676176807086" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2682" width="64" height="64" @click='showSide'>
                                        <path d="M117.418667 768h789.333333a32 32 0 0 1 4.352 63.701333l-4.352 0.298667h-789.333333a32 32 0 0 1-4.309334-63.701333L117.418667 768h789.333333-789.333333z m0-277.205333h789.333333a32 32 0 0 1 4.352 63.701333l-4.352 0.298667h-789.333333a32 32 0 0 1-4.309334-63.701334l4.309334-0.298666h789.333333-789.333333z m0-277.333334h789.333333a32 32 0 0 1 4.309333 63.701334l-4.352 0.298666h-789.333333A32 32 0 0 1 113.066667 213.76l4.309333-0.298667h789.333333-789.333333z" fill="#8176ff" p-id="2683"></path>
                                    </svg>
                                </div>
                            </div>
                        </div>
                        <div v-else>
                            <div class="row" style="width:100%">
                                <div class="col-5 text-start">
                                    <div class="img">
                                        <img style="height:8vh;width: 10vw;" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/logo-new@2x.png">
                                    </div>
                                </div>
                                <div class="col-7 text-end  mb-auto">
                                    <div class="row">
                                        <div class="col-8 text-center">
                                            <div class="navigation" style="height:100%">
                                                <div class="row " style="height:100%">
                                                    <div class="col-auto mx-auto my-auto" style="color:#8176ff">HOME</div>
                                                    <div class="col-auto mx-auto my-auto">ABOUT US</div>
                                                    <div class="col-auto mx-auto my-auto">SERVICE</div>
                                                    <div class="col-auto mx-auto my-auto">PAGES</div>
                                                    <div class="col-auto mx-auto my-auto">CONTACT US</div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="col-4 text-end">
                                            <div class="GetStart" style="padding:0px">
                                                <div class="row">
                                                    <div class="col" style="height: 100%;width: 100%;">
                                                        <button style="background: #8176FF;height: 100%;width: 100%;padding: 20px 30px ; border: 0px;border-radius: 50px;color: white;">GET STARTED</button>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="body">
                        <div class="easyPayment" style="width:100%;padding-top: 80px;padding-bottom: 80px;">
                            <div class="row">
                                <div class="col-12 col-md-6 text-start" style="padding:10px,20px,10px,10px;">
                                    <div class="description">
                                        <h1 class="title" style="padding-bottom: 20px;">
                                            <span style="color: #8176ff;">EASIEST</span>
                                            PAYMENT METHOD EVER
                                        </h1>
                                        <p class="text" style="padding-bottom: 20px;">QRPAY offers comprehensive digital payment services with a variety of payment options, making it a convenient solution for anyone seeking to collect payments electronically. It is secure, user-friendly, efficient, and does not require any additional hardware setup.</p>
                                        <div class="btn text-start">
                                            <button style="background: #8176FF;color: white;height: 60px; width:180px;border: 0px;border-radius: 50px;padding: 10px 15px ">GET STARTED</button>
                                            <button style="background: none;height: 60px;color:white; width:180px;border: 0px;border-radius: 50px;margin-left: 20px;">CONTACT US</button>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-12 col-md-6 text-end">
                                    <div class="img" style="padding:80px,10px,10px,40px;">
                                        <img style="width: 100%;height: 100%;" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/home-img-big@2x-e1609121743866.png">
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div ref="swiper" class="swiper" :slides-per-view="3">
                            <div class="swiper-wrapper" style="display: flex; ">
                                <div class="swiper-slide" v-for="icon in icons" :key="icon.image" style="padding: 55px;margin-left:15px ;width:200px;height:100px;">
                                    <li style="width: 175px;height: auto;"><img style="width:100%" :src="icon.image"></a></li>
                                </div>
                            </div>
                            <div class="swiper-autoplay"></div>
                            <div class="swiper-scrollbar"></div>
                        </div>
                        <div class="introduction" style="padding-top: 80px;padding-bottom: 80px;">
                            <div class="row">
                                <div class="col-12 col-md-6 text-start ">
                                    <div class="img">
                                        <img style="width:100%;height:100%" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/app-mockup-2-a@2x-e1610431074808.png">
                                    </div>
                                </div>
                                <div class="col-12 col-md-6 text-end" style="padding-left:50px;">
                                    <div class="description text-start" style="width:100%">
                                        <h1 class="title">
                                            Manage Everything in Your Hand
                                        </h1>
                                        <!-- <p class="text">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p> -->
                                        <div class="features">
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg>
                                                        </div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px 0px 10px 0px;">User Friendly</div>
                                                            <div class="text" id="1">
                                                                Convenience: QR codes provide a simple and fast way to receive payments, eliminating the need for physical cards, cash, or checkbooks.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">Best Support</div>
                                                            <div class="text" id="1">
                                                                Security: QR codes are encrypted and secure, reducing the risk of fraud and protecting sensitive information such as credit card numbers and bank account details.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">Secure</div>
                                                            <div class="text" id="1">
                                                                Wide Adoption: QR codes are widely used and recognized, making it easier for customers to make payments quickly and easily.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">4th</div>
                                                            <div class="text" id="1">
                                                                Contactless Payments: QR codes enable contactless payments, reducing the risk of exposure to viruses and other pathogens.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="introduction2" style="padding-top: 80px;padding-bottom: 80px;">
                            <div class="row">
                                <div class="col-12 col-md-6 text-end" style="padding-left:50px;">
                                    <div class="description text-start" style="width:100%">
                                        <h1 class="title">
                                            Manage Everything in Your Hand
                                        </h1>
                                        <!-- <p class="text">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p> -->
                                        <div class="features">
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg>
                                                        </div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px 0px 10px 0px;">5th</div>
                                                            <div class="text" id="1">
                                                                Reduced Costs: QR code payments can be processed without the need for additional hardware, reducing the costs associated with traditional payment methods.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">6th</div>
                                                            <div class="text" id="1">
                                                                Increased Sales: QR codes can increase sales by allowing merchants to receive payments from customers on the spot, without the need for time-consuming and error-prone manual processes. ***
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">7th</div>
                                                            <div class="text" id="1">
                                                                Data Tracking: QR codes can help merchants track sales and customer data, providing valuable insights into their business operations and performance.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                            <div class="mx-auto" style="padding:5px 10px 10px 10px">
                                                <div class="row" style="margin-bottom:20px;">
                                                    <div class="col-auto my-auto" style="margin-right: 30px;padding: 0px;">
                                                        <div class="logo1" style="background-color:#8176ff;border-radius: 50px;padding: 20px;"><svg t="1675940006814" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2685" width="60" height="60">
                                                                <path d="M704 128v768H320V128h384m0-64H320c-35.2 0-64 28.8-64 64v768c0 35.2 28.8 64 64 64h384c35.2 0 64-28.8 64-64V128c0-35.2-28.8-64-64-64zM272 192v64h480v-64H272z m0 576h480v-64H272v64z m176 96h128v-64H448v64z" p-id="2686" fill="#ffffff"></path>
                                                            </svg></div>
                                                    </div>
                                                    <div class="col my-auto">
                                                        <div class="description1" id="1">
                                                            <div class="subtitle" id="1" style="margin: 10px,0px,10px,0px;">8th</div>
                                                            <div class="text" id="1">
                                                                Environmental friendly: reducing paper waste, energy consumption, and carbon footprint, QR code payments contribute to a more sustainable and environmentally friendly future.
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-12 col-md-6 text-start ">
                                    <div class="img">
                                        <img style="width:100%;height:100%" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/app-mockup-2-a@2x-e1610431074808.png">
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="enjoyPro" style="padding-top: 80px;padding-bottom: 80px;">
                            <div class="row">
                                <div class="col-12 col-md-6 text-start">
                                    <div class="description" style="width:100%">
                                        <h1 class="title">
                                            Enjoy Various Merchant's Promos
                                        </h1>
                                        <p class="text">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
                                        <div class="btn text-start">
                                            <button style="background: #8176FF;color:white;height: 60px; width:180px;border: 0px;border-radius: 50px;padding: 10px 15px ">GET STARTED</button>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-12 col-md-6 text-end">
                                    <div id="ProsCard">
                                        <img style="width: 100%;height: auto;" src="../assets/back.png" alt="">
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="service" style="padding: 100px 0px 200px 0px;">
                            <div class="row">
                                <div class="col-12 text-center">
                                    <div class="description" style="width:100%;padding-bottom:40px">
                                        <h1 class="serviceTitle">
                                            Our Service
                                        </h1>
                                        <p class="serviceText">
                                            Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione.
                                        </p>
                                    </div>
                                </div>
                                <div class="col-12">
                                    <div class="cardsList">
                                        <div class="row" style="margin-top:40px">
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff;margin-bottom:16px;">Cash Flow Improvement</div>
                                                    <div class="cardDes" style="margin-bottom:10px">Receiving prepaid expenses can help improve the cash flow of a business by providing a source of revenue in advance.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff;margin-bottom:16px;">Reduced Risk</div>
                                                    <div class="cardDes">Prepaid expenses reduce the risk of non-payment for the merchant, as the customer has already paid for the goods or services.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff">Increased Customer Loyalty</div>
                                                    <div class="cardDes">Prepaid expenses can increase customer loyalty, as customers are more likely to return to a business where they have already made a commitment.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="row" style="margin-top:20px">
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff;margin-bottom:16px;">Improved Customer Experience</div>
                                                    <div class="cardDes">Offering prepaid options to customers can provide a more convenient and streamlined payment experience, which can increase customer satisfaction.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff;margin-bottom:16px;">Improved Planning</div>
                                                    <div class="cardDes"> Receiving prepaid expenses can allow merchants to plan and allocate resources more effectively, as they have a clearer understanding of their future revenue.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                            <div class="col-12 col-md-4">
                                                <div class="cardContent" style="background-color: #1F1B41;border-radius: 20px;padding: 30px;margin-left: 20px;margin-right: 20px;">
                                                    <div class="cardLogo" style="padding-bottom: 20px;">
                                                        <svg t="1675945988703" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3273" width="40" height="40">
                                                            <path d="M841.704141 99.863429l-659.418514 0c-45.51666 0-82.417081 36.910655-82.417081 82.437547l0 659.408281c0 45.51666 36.900422 82.427314 82.417081 82.427314l659.418514 0c45.526893 0 82.427314-36.910655 82.427314-82.427314l0-659.408281C924.131455 136.774083 887.231033 99.863429 841.704141 99.863429zM718.058053 429.572686l0 82.427314L553.213657 512l0 82.427314 164.844395 0 0 82.417081L553.213657 676.844395l0 123.646088-82.427314 0 0-123.646088-164.854629 0 0-82.417081 164.854629 0 0-82.427314-164.854629 0 0-82.427314 178.024579 0-219.243353-206.052936 123.646088 0 123.635855 123.625622 123.646088-123.625622 123.635855 0-210.801077 206.052936L718.058053 429.572686z" p-id="3274" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="cardTitle" style="color:#8176ff;margin-bottom:16px;">Reduced Costs</div>
                                                    <div class="cardDes"> By receiving prepaid expenses, merchants can reduce the costs associated with chasing payments and minimize the risk of bad debt.
                                                    </div>
                                                    <div class="cardNav" style="color:#8176ff;margin-top:20px;">Learn More</div>
                                                </div>
                                            </div>
                                            <div class="col-12 col-md-4 text-center ">
                                                <div class="viewMore " style="margin-left: 20px;margin-right: 20px;padding:30px;height: 100%;">
                                                    <div class="viewContent" style="height:100%">
                                                        <div class="row " style="height:100%">
                                                            <div class="col my-auto">
                                                                <p class="viewMore_text " style="margin-bottom: 15px;padding-bottom: 0px;">
                                                                    We have a lot of powerful service that you can get. Check for more of our available services in our product.
                                                                </p>
                                                                <div class="viewMore_btn">
                                                                    <button style="background-color:#6B5EFF;border: 0px;border-radius: 50px;padding: 20px 30px;color: white;">VIEW MORE</button>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="profileCard " style="padding:50px 0px 50px 0px">
                            <div class="row">
                                <div class="col-12">
                                    <div class="profileBackground">
                                        <div class="row">
                                            <div class="col text-center"><img style="width:100px;height:100px;" src="../assets/profileIcon.png" alt=""></div>
                                        </div>
                                        <div class="row" style="padding-bottom: 70px;padding-top: 50px;">
                                            <div class="col">
                                                <div class="profileContent">
                                                    <div class="row ">
                                                        <div class="col-6 mx-auto text-center">
                                                            <p class="des"> Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
                                                        </div>
                                                    </div>
                                                    <div class="row ">
                                                        <div class="col ">
                                                            <div class="profileInfo d-flex ">
                                                                <div class="mx-auto ">
                                                                    <div class="row">
                                                                        <div class="col">
                                                                            <img src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2021/01/testi-foto@2x@2x-e1610431253715.jpg" style="width:100px;height:100px;border-radius: 50px;">
                                                                        </div>
                                                                        <div class="col my-auto">
                                                                            <div class="name" style="color:#151518;">Jane Daya</div>
                                                                            <div class="position">customer</div>
                                                                        </div>
                                                                    </div>
                                                                </div>
                                                            </div>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="easyPaymentInfo" style="padding:150px 0px 100px 0px">
                            <div class="row">
                                <div class="col-12 col-md-6 text-start">
                                    <div class="description" style="width:100%;height:100%;">
                                        <h1 class="title" style="margin-bottom:20px;">
                                            Support Payment From Every Plartform
                                        </h1>
                                        <p class="text" style="margin-bottom:20px;">Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
                                        <div class="supportedPayment">
                                            <div class="row" style="margin-bottom:20px;">
                                                <div class="col">Supported Payment :</div>
                                            </div>
                                            <div class="row">
                                                <div class="col-auto" style="background-color:#8176FF;border-radius:5px;margin-right: 20px;">
                                                    <svg t="1675945263726" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="14578" width="48" height="48">
                                                        <path d="M483.981653 769.322667c2.474667 2.090667 5.12 4.181333 7.722667 6.229333a315.349333 315.349333 0 0 1-175.232 52.821333 316.416 316.416 0 1 1 175.104-579.968c-2.56 2.176-5.12 4.181333-7.04 6.4A339.754667 339.754667 0 0 0 366.733653 512a341.162667 341.162667 0 0 0 117.248 257.322667z m223.616-573.738667c-64.853333 0-125.056 19.456-175.146666 52.821333 2.56 2.176 5.12 4.181333 7.04 6.4A339.754667 339.754667 0 0 1 657.293653 512a341.418667 341.418667 0 0 1-117.248 257.322667c-2.474667 2.090667-5.12 4.181333-7.722666 6.229333a315.136 315.136 0 0 0 175.232 52.821333A316.330667 316.330667 0 0 0 1024.013653 512a316.458667 316.458667 0 0 0-316.416-316.416zM512.013653 263.424A315.221333 315.221333 0 0 0 391.22432 512 315.136 315.136 0 0 0 512.013653 760.618667 315.306667 315.306667 0 0 0 632.802987 512 315.221333 315.221333 0 0 0 512.013653 263.424z" p-id="14579"></path>
                                                    </svg>
                                                </div>
                                                <div class="col-auto" style="background-color:#8176FF;border-radius:5px;margin-right: 20px;margin-left:20px;">
                                                    <svg t="1675945724469" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="15546" width="64" height="64">
                                                        <path d="M868.957 192.158H155.043c-49.958 0-90.604 40.645-90.604 90.604v458.477c0 49.958 40.645 90.604 90.604 90.604h713.914c49.958 0 90.604-40.646 90.604-90.604V282.762c0-49.959-40.646-90.604-90.604-90.604z m27.29 549.08c0 15.048-12.242 27.29-27.29 27.29H155.043c-15.048 0-27.29-12.242-27.29-27.29V282.762c0-15.048 12.242-27.29 27.29-27.29h713.914c15.048 0 27.29 12.242 27.29 27.29v458.476z" p-id="15547" fill="#1F1B41"></path>
                                                        <path d="M298.044 519.641l-24.015-120.077H153.952s96.061 24.015 144.092 120.077z" p-id="15548" fill="#1F1B41"></path>
                                                        <path d="M359.174 399.564l-54.581 157.192-4.366-21.832s-21.832-58.947-78.596-93.879l45.848 181.207h63.313l89.512-222.689c0.001 0.001-60.038 0.001-61.13 0.001zM409.389 620.069h58.947l34.931-220.505H444.32zM595.024 477.766c-4.384-2.305-10.743-5.113-11.867-6.985-0.14-0.233-0.236-0.859-0.356-1.942-1.425-12.88 2.373-16.016 3.625-17.046 12.566-10.355 53.048-5.324 77.43 2.292l15.071-47.901c-14.01-4.418-85.854-24.855-124.373 6.806-11.905 9.786-25.327 28.38-21.66 61.392 3.239 29.149 22.935 39.507 38.759 47.828 11.948 6.281 25.476 13.396 42.183 29.981 1.588 2.512 4.622 11.552 1.087 16.922-5.238 7.963-32.126 17.442-99.659 2.431l-10.895 49.02c27.363 6.078 51.38 9.115 72.002 9.115 41.616 0 69.405-12.362 82.933-37.004 15.27-27.815 4.309-61.723-9.473-75.505-22.323-22.322-41.872-32.603-54.807-39.404zM763.071 399.564L668.1 621.161h56.764l12.008-31.657h74.23l6.55 30.565h52.397l-43.664-220.505h-63.314z m-9.825 147.368l32.748-85.146c0.819-0.819 17.466 85.146 17.466 85.146h-50.214z" p-id="15549" fill="#1F1B41"></path>
                                                    </svg>
                                                </div>
                                                <div class="col-auto" style="background-color:#8176FF;border-radius:5px;margin-right: 20px;margin-left:20px;">
                                                    <svg t="1675945847983" class="icon" viewBox="0 0 1316 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1412" width="64" height="64">
                                                        <path d="M425.714286 517.714286q0 21.142857-14.571429 35.142857T375.428571 566.857143q-16.571429 0-26.571428-9.142857T338.857143 532.571429q0-21.142857 14.285714-35.714286t35.428572-14.571429q16 0 26.571428 9.428572T425.714286 517.714286z m448.571428-85.142857q0 24-12.571428 32.571428t-37.714286 8.571429l-18.285714 0.571428 9.714285-61.142857q1.142857-6.285714 7.428572-6.285714h10.285714q12.571429 0 20 1.142857t14.285714 7.142857 6.857143 17.428572z m200.571429 85.142857q0 20.571429-14.571429 34.857143t-35.142857 14.285714q-16.571429 0-26.857143-9.142857t-10.285714-25.142857q0-21.142857 14.285714-35.714286t35.428572-14.571429q16 0 26.571428 9.428572T1074.857143 517.714286zM293.142857 420q0-33.714286-22-48.857143T213.714286 356H122.285714q-10.857143 0-12 10.857143l-37.142857 233.142857q-0.571429 3.428571 1.714286 6.285714t5.714286 2.857143h43.428571q11.428571 0 12.571429-10.857143L146.857143 535.428571q0.571429-4.571429 4-7.428571t8.571428-3.714286 9.714286-0.857143 10.857143 0.571429 8 0.571429q49.142857 0 77.142857-27.714286T293.142857 420z m176.571429 178.285714l23.428571-149.142857q0.571429-3.428571-1.714286-6.285714t-5.714285-2.857143h-43.428572q-8 0-9.714285 18.857143-15.428571-22.857143-54.285715-22.857143-41.142857 0-70 30.857143T279.428571 539.428571q0 33.714286 19.714286 53.714286t52.857143 20q16 0 33.142857-6.857143t27.428572-18.285714q-2.285714 6.857143-2.285715 12 0 9.142857 7.428572 9.142857h39.428571q10.857143 0 12.571429-10.857143z m255.428571-150.285714q0-2.857143-2.285714-5.428571t-5.142857-2.571429h-44q-6.285714 0-10.285715 5.714286L602.857143 534.857143l-25.142857-85.714286q-2.857143-9.142857-12.571429-9.142857h-42.857143q-2.857143 0-5.142857 2.571429t-2.285714 5.428571q0 1.142857 11.142857 33.714286t24 70.285714 13.428571 40q-46.857143 64-46.857142 68.571429 0 7.428571 7.428571 7.428571h44q6.285714 0 10.285714-5.714286l145.714286-210.285714q1.142857-1.142857 1.142857-4z m217.142857-28q0-33.714286-22-48.857143T862.857143 356h-90.857143q-11.428571 0-12.571429 10.857143l-37.142857 233.142857q-0.571429 3.428571 1.714286 6.285714t5.714286 2.857143h46.857143q6.857143 0 9.142857-7.428571l10.285714-66.285715q0.571429-4.571429 4-7.428571t8.571429-3.714286 9.714285-0.857143 10.857143 0.571429 8 0.571429q49.142857 0 77.142857-27.714286t28-76.857143z m176.571429 178.285714l23.428571-149.142857q0.571429-3.428571-1.714285-6.285714t-5.714286-2.857143h-43.428572q-8 0-9.714285 18.857143-14.857143-22.857143-54.285715-22.857143-41.142857 0-70 30.857143T928.571429 539.428571q0 33.714286 19.714285 53.714286t52.857143 20q16.571429 0 33.714286-6.857143t26.857143-18.285714q0 0.571429-1.142857 5.142857t-1.142858 6.857143q0 9.142857 7.428572 9.142857h39.428571q10.857143 0 12.571429-10.857143z m124.571428-233.714285v-0.571429q0-8-7.428571-8h-42.285714q-6.285714 0-7.428572 6.285714l-37.142857 237.714286-0.571428 1.142857q0 2.857143 2.285714 5.428572t5.714286 2.571428h37.714285q10.857143 0 12-10.857143zM224 441.142857q-2.857143 20-14.857143 26.285714t-34.285714 6.285715l-18.857143 0.571428 9.714286-61.142857q1.142857-6.285714 7.428571-6.285714h10.857143q22.857143 0 33.142857 6.571428t6.857143 27.714286z m1092.571429-294.857143v731.428572q0 29.714286-21.714286 51.428571t-51.428572 21.714286H73.142857q-29.714286 0-51.428571-21.714286t-21.714286-51.428571V146.285714q0-29.714286 21.714286-51.428571t51.428571-21.714286h1170.285714q29.714286 0 51.428572 21.714286t21.714286 51.428571z" p-id="1413"></path>
                                                    </svg>
                                                </div>
                                                <div class="col-auto" style="background-color:#8176FF;border-radius:5px;margin-right: 20px;margin-left:20px;">
                                                    <svg t="1675945887316" class="icon" viewBox="0 0 1280 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2104" width="64" height="64">
                                                        <path d="M1280 523.2c0-91-44-162.8-128.4-162.8s-135.8 71.8-135.8 162.2c0 107 60.6 156.4 147 156.4 42.4 0 74.2-9.6 98.4-23v-66.8c-24.2 12.2-52 19.6-87.2 19.6-34.6 0-65-12.2-69-53.8h173.8c0.4-4.6 1.2-23.2 1.2-31.8m-175.8-33.6c0-40 24.6-56.8 46.8-56.8 21.8 0 45 16.8 45 56.8h-91.8z m-225.8-129.2c-34.8 0-57.2 16.4-69.6 27.8l-4.6-22H726v409.6l88.8-18.8 0.2-100.4c12.8 9.4 31.8 22.4 62.8 22.4 63.6 0 121.6-46.4 121.6-159.2 0.2-103.2-58.6-159.4-121-159.4m-21.2 245c-20.8 0-33.2-7.6-41.8-16.8l-0.6-132c9.2-10.2 22-17.6 42.4-17.6 32.4 0 54.8 36.4 54.8 82.8 0.2 47.8-21.8 83.6-54.8 83.6M692.8 248v72.4l-89.2 19v-72.4l89.2-19m-89 118.4h89.2v306.4h-89.2V366.4z m-95.6 26.2c20.8-38.2 62.2-30.4 74.2-26.2V448c-11.4-3.6-46.8-9-67.8 18.6v206.2H426V366.4h76.8l5.4 26.2m-178-26.2h67.4V442h-67.4v126.4c0 52.4 56 36 67.4 31.4v67.6c-11.8 6.4-33.2 11.8-62.4 11.8-52.6 0-92.2-34-92.2-86.6l0.4-284.8 86.6-18.4 0.2 77zM89.8 456.6c0 40 135.8 21 135.8 126.8 0 64-50.8 95.6-124.6 95.6-30.6 0-64-6-97-20.2v-80c29.8 16.2 67.8 28.4 97.2 28.4 19.8 0 34-5.4 34-21.8 0-42.4-135-26.4-135-124.8 0-62.8 48-100.4 120-100.4 29.4 0 58.8 4.6 88.2 16.2V460c-27-14.6-61.4-22.8-88.4-22.8-18.6 0.2-30.2 5.6-30.2 19.4" fill="#1F1B41" p-id="2105"></path>
                                                    </svg>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-6 text-end">
                                    <div class="paymentInfoCard">
                                        <div class="womenImg">
                                            <img style="width: 100%;height: auto;" src="../assets/card2.png" alt="">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="updated" style="padding:50px 0px 50px 0px;padding:60px;border-radius: 30px;margin-bottom: 50px;">
                            <div class="row">
                                <h2 class="col-12 col-md-6 text-start">
                                    Keep Updated About Our Product
                                </h2>
                                <div class="col-12 col-md-6 text-center my-auto" style="width
                                            :100%;height:100%">
                                    <div class="input-group mb-3" style="width
                                            :100%;height:100%">
                                        <input type="text" class="form-control" placeholder="Your email address" aria-label=" users' email address" aria-describedby="basic-addon2" style="border-radius: 50px;">
                                        <div class="input-group-append">
                                            <button class="btn btn-outline-secondary" type="button" style="border-radius: 50px;">Submit</button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="footer h-100">
                        <div class="row ">
                            <div class="col-12 col-md-3 text-start" style="padding: 10px,60px,10px,10px;">
                                <div class="row" style="padding-bottom:20px">
                                    <div class="col-auto text-start">
                                        <div class="img">
                                            <img style="height:8vh;width: 10vw;" src="https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/logo-new@2x.png">
                                        </div>
                                    </div>
                                </div>
                                <div class="row" style="padding-bottom:20px">
                                    <div class="col-auto text-start">One Application for Every Payment</div>
                                </div>
                                <div class="row">
                                    <div class="col-auto text-start"><svg t="1675941625663" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3689" width="50" height="50">
                                            <path d="M747.4 535.7c-0.4-68.2 30.5-119.6 92.9-157.5-34.9-50-87.7-77.5-157.3-82.8-65.9-5.2-138 38.4-164.4 38.4-27.9 0-91.7-36.6-141.9-36.6C273.1 298.8 163 379.8 163 544.6c0 48.7 8.9 99 26.7 150.8 23.8 68.2 109.6 235.3 199.1 232.6 46.8-1.1 79.9-33.2 140.8-33.2 59.1 0 89.7 33.2 141.9 33.2 90.3-1.3 167.9-153.2 190.5-221.6-121.1-57.1-114.6-167.2-114.6-170.7z" p-id="3690" fill="#8176ff"></path>
                                            <path d="M642.3 230.7c50.7-60.2 46.1-115 44.6-134.7-44.8 2.6-96.6 30.5-126.1 64.8-32.5 36.8-51.6 82.3-47.5 133.6 48.4 3.7 92.6-21.2 129-63.7z" p-id="3691" fill="#8176ff"></path>
                                        </svg>
                                    </div>
                                    <div class="col-auto text-start"><svg t="1675943038098" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="4559" width="50" height="50">
                                            <path d="M708.266667 669.866667l213.333333-123.733334c8.533333-4.266667 17.066667-17.066667 17.066667-25.6v-12.8c0-12.8-4.266667-21.333333-17.066667-25.6l-213.333333-123.733333-140.8 153.6 140.8 157.866667z m-174.933334-196.266667l128-145.066667L187.733333 46.933333c-8.533333-4.266667-17.066667-4.266667-25.6 0l371.2 426.666667z m0 81.066667L162.133333 981.333333c8.533333 4.266667 17.066667 4.266667 25.6 0l473.6-277.333333-128-149.333333zM128 89.6v844.8l371.2-422.4L128 89.6z" p-id="4560" fill="#8176ff"></path>
                                        </svg>
                                        </svg>
                                    </div>
                                    <div class="col-auto text-start"><svg t="1675941625663" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3689" width="50" height="50">
                                            <path d="M747.4 535.7c-0.4-68.2 30.5-119.6 92.9-157.5-34.9-50-87.7-77.5-157.3-82.8-65.9-5.2-138 38.4-164.4 38.4-27.9 0-91.7-36.6-141.9-36.6C273.1 298.8 163 379.8 163 544.6c0 48.7 8.9 99 26.7 150.8 23.8 68.2 109.6 235.3 199.1 232.6 46.8-1.1 79.9-33.2 140.8-33.2 59.1 0 89.7 33.2 141.9 33.2 90.3-1.3 167.9-153.2 190.5-221.6-121.1-57.1-114.6-167.2-114.6-170.7z" p-id="3690" fill="#8176ff"></path>
                                            <path d="M642.3 230.7c50.7-60.2 46.1-115 44.6-134.7-44.8 2.6-96.6 30.5-126.1 64.8-32.5 36.8-51.6 82.3-47.5 133.6 48.4 3.7 92.6-21.2 129-63.7z" p-id="3691" fill="#8176ff"></path>
                                        </svg>
                                    </div>
                                </div>
                            </div>
                            <div class="col-auto col-md-9">
                                <div class="row">
                                    <div class="col-12 col-md-3 text-start">
                                        <div class="otherPages" style="padding:10px">
                                            <div class="col-auto">
                                                <div class="footerTitle">
                                                    <div class="row" style="padding-bottom:20px">
                                                        <div class="col">Other Pages</div>
                                                    </div>
                                                </div>
                                                <div class="footerText">
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Home</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">About Us</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Services</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Contact</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Project</div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-12 col-md-3 text-start">
                                        <div class="quickLinks" style="padding:10px">
                                            <div class="col-auto">
                                                <div class="footerTitle">
                                                    <div class="row" style="padding-bottom:20px">
                                                        <div class="col">Quick Links</div>
                                                    </div>
                                                </div>
                                                <div class="footerText">
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Privacy Policy
                                                        </div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Term Of Service</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Disclaimer
                                                        </div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Credits</div>
                                                    </div>
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">FAQ</div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="col-12 col-md-6 text-start">
                                        <div class="socialMedia" style="padding:10px;">
                                            <div class="col-auto">
                                                <div class="footerTitle">
                                                    <div class="row" style="padding-bottom:20px">
                                                        <div class="col">Social Media</div>
                                                    </div>
                                                </div>
                                                <div class="footerText">
                                                    <div class="row" style="padding-bottom:10px">
                                                        <div class="col">Our Support and Sales team is available 24 /7 to answer your queries</div>
                                                    </div>
                                                </div>
                                                <div class="row" style="padding-bottom:10px">
                                                    <div class="col-auto text-start"><svg t="1675944578646" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="9307" width="32" height="32">
                                                            <path d="M880 112H144c-17.7 0-32 14.3-32 32v736c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V144c0-17.7-14.3-32-32-32z m-92.4 233.5h-63.9c-50.1 0-59.8 23.8-59.8 58.8v77.1h119.6l-15.6 120.7h-104V912H539.2V602.2H434.9V481.4h104.3v-89c0-103.3 63.1-159.6 155.3-159.6 44.2 0 82.1 3.3 93.2 4.8v107.9z" p-id="9308" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="col-auto ">
                                                        <svg t="1675944379181" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="6310" width="30" height="30">
                                                            <path d="M928 254.3c-30.6 13.2-63.9 22.7-98.2 26.4 35.4-21.1 62.3-54.4 75-94-32.7 19.5-69.7 33.8-108.2 41.2C765.4 194.6 721.1 174 672 174c-94.5 0-170.5 76.6-170.5 170.6 0 13.2 1.6 26.4 4.2 39.1-141.5-7.4-267.7-75-351.6-178.5-14.8 25.4-23.2 54.4-23.2 86.1 0 59.2 30.1 111.4 76 142.1-28-1.1-54.4-9-77.1-21.7v2.1c0 82.9 58.6 151.6 136.7 167.4-14.3 3.7-29.6 5.8-44.9 5.8-11.1 0-21.6-1.1-32.2-2.6C211 652 273.9 701.1 348.8 702.7c-58.6 45.9-132 72.9-211.7 72.9-14.3 0-27.5-0.5-41.2-2.1C171.5 822 261.2 850 357.8 850 671.4 850 843 590.2 843 364.7c0-7.4 0-14.8-0.5-22.2 33.2-24.3 62.3-54.4 85.5-88.2z" p-id="6311" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                    <div class="col-auto"><svg t="1675944379181" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="6310" width="30" height="30">
                                                            <path d="M928 254.3c-30.6 13.2-63.9 22.7-98.2 26.4 35.4-21.1 62.3-54.4 75-94-32.7 19.5-69.7 33.8-108.2 41.2C765.4 194.6 721.1 174 672 174c-94.5 0-170.5 76.6-170.5 170.6 0 13.2 1.6 26.4 4.2 39.1-141.5-7.4-267.7-75-351.6-178.5-14.8 25.4-23.2 54.4-23.2 86.1 0 59.2 30.1 111.4 76 142.1-28-1.1-54.4-9-77.1-21.7v2.1c0 82.9 58.6 151.6 136.7 167.4-14.3 3.7-29.6 5.8-44.9 5.8-11.1 0-21.6-1.1-32.2-2.6C211 652 273.9 701.1 348.8 702.7c-58.6 45.9-132 72.9-211.7 72.9-14.3 0-27.5-0.5-41.2-2.1C171.5 822 261.2 850 357.8 850 671.4 850 843 590.2 843 364.7c0-7.4 0-14.8-0.5-22.2 33.2-24.3 62.3-54.4 85.5-88.2z" p-id="6311" fill="#8176ff"></path>
                                                        </svg></div>
                                                    <div class="col-auto">
                                                        <svg t="1675944510765" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="8236" width="32" height="32">
                                                            <path d="M512 306.9c-113.5 0-205.1 91.6-205.1 205.1S398.5 717.1 512 717.1 717.1 625.5 717.1 512 625.5 306.9 512 306.9z m0 338.4c-73.4 0-133.3-59.9-133.3-133.3S438.6 378.7 512 378.7 645.3 438.6 645.3 512 585.4 645.3 512 645.3zM725.5 250.7c-26.5 0-47.9 21.4-47.9 47.9s21.4 47.9 47.9 47.9 47.9-21.3 47.9-47.9c-0.1-26.6-21.4-47.9-47.9-47.9z" p-id="8237" fill="#8176ff"></path>
                                                            <path d="M911.8 512c0-55.2 0.5-109.9-2.6-165-3.1-64-17.7-120.8-64.5-167.6-46.9-46.9-103.6-61.4-167.6-64.5-55.2-3.1-109.9-2.6-165-2.6-55.2 0-109.9-0.5-165 2.6-64 3.1-120.8 17.7-167.6 64.5C132.6 226.3 118.1 283 115 347c-3.1 55.2-2.6 109.9-2.6 165s-0.5 109.9 2.6 165c3.1 64 17.7 120.8 64.5 167.6 46.9 46.9 103.6 61.4 167.6 64.5 55.2 3.1 109.9 2.6 165 2.6 55.2 0 109.9 0.5 165-2.6 64-3.1 120.8-17.7 167.6-64.5 46.9-46.9 61.4-103.6 64.5-167.6 3.2-55.1 2.6-109.8 2.6-165z m-88 235.8c-7.3 18.2-16.1 31.8-30.2 45.8-14.1 14.1-27.6 22.9-45.8 30.2C695.2 844.7 570.3 840 512 840c-58.3 0-183.3 4.7-235.9-16.1-18.2-7.3-31.8-16.1-45.8-30.2-14.1-14.1-22.9-27.6-30.2-45.8C179.3 695.2 184 570.3 184 512c0-58.3-4.7-183.3 16.1-235.9 7.3-18.2 16.1-31.8 30.2-45.8s27.6-22.9 45.8-30.2C328.7 179.3 453.7 184 512 184s183.3-4.7 235.9 16.1c18.2 7.3 31.8 16.1 45.8 30.2 14.1 14.1 22.9 27.6 30.2 45.8C844.7 328.7 840 453.7 840 512c0 58.3 4.7 183.2-16.2 235.8z" p-id="8238" fill="#8176ff"></path>
                                                        </svg>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="row">
                            <div class="col">
                                <div class="divider" style="margin-bottom: 20px;margin-top: 40px; background:grey;"> </div>
                            </div>
                        </div>
                        <div class="row" style="padding:10px">
                            <div class="col-auto text-start">Company Name</div>
                            <div class="col text-end">Copyright</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    // @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import sidebar from '@/components/SideBar.vue'
import Swiper, {Autoplay } from 'swiper'
import 'swiper/css'

import 'swiper/css/autoplay'




 
  





export default  {
    name: 'HomeView',

    components: {
        HelloWorld,
         Swiper,
         sidebar,
      
    },
    data(){
      return{
        icons:[
          {"image":"https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/global-trade-logo@2x.png"},
          {"image":"https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/marketup-logo@2x.png"},
          {"image":"https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/okfinance-logo@2x.png"},
          {"image":"https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/marketchat-logo@2x.png"},
          {"image":"https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2020/12/starbank-logo@2x.png"},
          ],
        showSideBar:false,
       

      



      }
    },
    created() {
    // Use in js
    console.log(this.$isMobile());
  },
  
    mounted(){
      new Swiper(this.$refs.swiper, {
      // configure Swiper to use modules
      modules: [Autoplay],
      // Optional parameters
      loop: false,
      slidesPerView: 4,

      // If we need pagination
     

      // Navigation arrows
      

      // And if we need scrollbar
      scrollbar: {
        el: '.swiper-scrollbar',
        draggable: true,
    dragSize: 100,
      },
       
      autoplay:{
        el:'.swiper-autoplay',
      }
    })
    },
    methods:{
        showSide(){
            this.showSideBar=true;
            console.log(this.showSideBar)

        },
        closeSidebar() {
            this.showSideBar = false
        }
       
    }
    
}
</script>
<style type="text/css">
.home {
    background-color: #151518;

    background-repeat: no-repeat;









    background-size: cover;
}

.swiper-wrapper {
    display: flex;


}

.swiper-slide {
    padding: 60px;
    margin-right: 15px;
}

/*.sw {
  width: 94%;
  height: 2rem;
  text-align: center;
}
.sw img {
  height: auto;
  width: 100%;
}*/

.wrapper {
    color: white;
}


.GetStart {
    background-image: linear-gradient(60deg, #6B5EFF 0%, var(--e-global-color-335476e) 82%);

}

.description {
    padding-left: 0px;

    margin: 0;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    transform: translateY(-50%);

}

.viewMore {
    margin: 0;
    height: 100%;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    transform: translateY(-50%);
}




.navigation {
    font-family: "Montserrat", Sans-serif;
    font-size: 14px;
    font-weight: 500;
}

.btn {
    color: white;
    background-image: linear-gradient(60deg, #6B5EFF 0%, var(--e-global-color-335476e) 82%);
    padding: 0px;

}

.viewMore_btn {
    color: white;
    background-image: linear-gradient(60deg, #6B5EFF 0%, var(--e-global-color-335476e) 82%);

}

.title {
    font-size: 60px;
}

.text {
    font-size: 18px;
}

.subtitle {
    margin: 10px 0px 10px 0px;
    padding: 0px 0px 0px 0px;
    color: #8176ff;
    font-family: var(--e-global-typography-4dab1ce-font-family), Sans-serif;

    font-size: 18px;
}

.cardsList {

    background-image: radial-gradient(at top right, #1F1B41 0%, var(--e-global-color-8f64ec5) 70%);
}

.cardTitle {
    color: var(--e-global-color-335476e);
}

.cardNav {
    color: var(--e-global-color-335476e);
}

#ProsCard {
    background-image: url("https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2021/01/shopping-girl-home1@2x.jpg");

    position: relative;
    background-size: cover;
    background-repeat: no-repeat;
}

.profileBackground {
    width: 100%;
    height: auto;
    /*position: relative;
    top: 50%;
    transform: translateY(-50%);
    transform: translateY(-50%);*/


    background-image: url("https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2021/01/testi-bg@2x.png");
    background-color: #1C1B1B00;
    background-size: contain;
    background-repeat: no-repeat;



}


.profileInfo {
    margin: 0;
    position: relative;
    left: 50%;
    transform: translateX(-50%);
    transform: translateX(-50%);
}

.paymentInfoCard {
    background-image: url("https://templatekit.jegtheme.com/izpay/wp-content/uploads/sites/30/2021/01/payment-img@2x.jpg");

    position: relative;
    background-size: cover;
    background-repeat: no-repeat;
}

.updated {
    background-image: linear-gradient(210deg, #8176ff 0%, #6b5eff 100%);
}



.footer {
    margin-top: 50px;
    color: white;
}

.footerTitle {

    color: #8176ff;
    font-family: "Montserrat", Sans-serif;
    font-size: 18px;
    font-weight: 600;
}

.footerText {
    color: var(--e-global-color-335476e);
    font-family: var(--e-global-typography-text-font-family), Sans-serif;
    font-size: var(--e-global-typography-text-font-size);
    font-weight: var(--e-global-typography-text-font-weight);
}

.divider {
    text-align: center;
    padding-top: 2px;
    padding-bottom: 2px;

}
</style>
<template>

    <div class="Footer">
        <footer>
            <div class="SocialMedia">
                <div class="Facebook">
                    <i class="fa-brands fa-facebook-f"></i>
                </div>
                <div class="Twitter">
                     <i class="fa-brands fa-twitter"></i>
                </div>
                <div class="Linkedin">
                    <i class="fa-brands fa-linkedin"></i>
                </div>
            </div>
            
        </footer>
    </div>
</template>

<style scoped>
    footer {
        height: 100%;
        width: 100%;
  }
   .SocialMedia {
        
        height: 70%;
        display: flex;
        justify-content: space-around;
        
        position: relative;
        top: 2rem;
        
        /* Position des icônes au centre */
        text-align: center;
        line-height: 140px;
        font-size: 3rem;
        color: white;
        
   }

   .Facebook {
       
        width: 30%;
        border-radius: 4px;
        background-color: #3b5998;  
        cursor: pointer;   
   }


   .Twitter {
       
        width: 30%;
        border-radius: 4px;
        background-color: #01aced;
        cursor: pointer;
   }

   .Linkedin {
       
        width: 30%;
        border-radius: 4px;
        background-color: #4875b4;
        cursor: pointer;
   }

</style>
 
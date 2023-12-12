<template>
    <div class="border1px">

        <h1>Home</h1>
        <h5>Name : {{name}}</h5>
        <h6>Full Name : {{getName("Prajkta Haadole") }}</h6>
        <h6>Email : {{ email }}</h6>
        <h6>Property : {{ 10+15+ 50 }}Cr</h6>
        <h6>Mobile : {{mobile}}</h6>
        <h6>Mobile : {{mobile=11111111}}</h6>          
         <!-- this value we can assigned and change in template by interpolation -->
        <h6>Mobile : {{mobile==11111111}}</h6>
        <h6>Age : {{getAge()}} Years</h6> 
        <h6> family details : 
            [ Father Name :{{ getparentDetails().fatherName}},
            <br>
              Mother Name :{{ getparentDetails().motherName}},
              <br>
              Sister Name :{{ getSiblingsDetails().sisterName}},
              <br>
              Brother Name :{{ getSiblingsDetails().brotherName}},
              <br>
                conatactId : {{ getparentDetails().email }}
                <!-- RETURN SAME contact ID   -->
            ]</h6> 

       
    </div>
   
</template>
<script>

export default {
    name : "Home",
    data(){
        return {
            technologies : ["javascript", "java", "python"],
            name : "Prajakta",
            email: "prajaktahadole@gmail.com",
            mobile: 874185296,
            getName : function(x){
                return x;
            },
           
        }
    },

    methods : {
        getAge(){
          return 22;
      },

      getparentDetails(){
          return {
                fatherName : "Vijay Hadole",
                motherName : "Jaya Hadole",
                email : this.email,
            };
      },
      getSiblingsDetails(){
        return {
            sisterName: "Sakshi Hadole",
            brotherName : "Parth Hadole",
        }
      },

      getOtherDetails (){
        return {
            nation : 'India',
            maritailStatus : "Single",

        }
      }
      
    },

}

</script>

<style scoped>
.border1px{
    border: 5px solid red;
    padding: 15px;
    margin: auto;
}

</style>
<template>
   <div class="Aside">
      <div class="Location">
         <h3>Location</h3>
         <el-select v-model="value" placeholder="選擇地區">
            <el-option v-for="item in options" :key="item.value" :value="item.value" :label="item.label">
            </el-option>
         </el-select>
      </div>
      <div class="Date">
         <h3>Date</h3>
         <div class="from">
            <span>from</span>
            <el-date-picker v-model="date_from" value-format="yyyy/MM/dd" />
         </div>
         <div class="to">
            <span>to</span>
            <el-date-picker v-model="date_to" value-format="yyyy/MM/dd" />
         </div>
      </div>
      <div class="Categories">
         <h3>Categories</h3>
         <el-checkbox-group v-model="checkList">
            <el-checkbox label="All"></el-checkbox>
            <el-checkbox label="Entertainment"></el-checkbox>
            <el-checkbox label="Food"></el-checkbox>
            <el-checkbox label="Learning"></el-checkbox>
            <el-checkbox label="Outdoors"></el-checkbox>
         </el-checkbox-group>

      </div>
   </div>
</template>

<style lang="scss">
   .Aside {
      background-color: #ebebeb;
		// max-width: 300px;
		width: 100%;
      padding: 0 40px;


      display: inline-flex;
      flex-direction: column;
      justify-content: flex-start;
      h3 {
         font-size: 20px;
         margin: 0;
         margin-bottom: 15px;
      }
      .Location, .Date, .Categories{
         padding-bottom: 24px;
         padding-top: 24px;
         border-bottom: 1px solid #D7D7D7;
         font-size: 16px;

         .el-input{
				min-width: 169px;
				width: 100%;
            height: 40px;
         }
         .el-checkbox{
            display: block;
            margin-left: 0;
            font-weight: 400;
            color: black;
            // &.el-checkbox{
            //    margin: 0;
            // }
         }
         &:last-child{
            border-bottom: none;
         }
      }
      .Date{
         .from, .to{
				width: 100%;
            display: flex;
            align-items: center;
            justify-content: flex-end;
            margin-bottom: 8px;

            &:last-child{
               margin-bottom: 0;
            }
            span{
               font-size: 16px;
               margin-right: 13px;
            }
            .el-date-editor{
               width: 169px;
               height: 40px;
               display: inline-block;
            }

         }
      }

   }
</style>

<script>
   export default {
      data() {
         return {
            value: '',
            date_from: '',
            date_to: '',
            options: [{
               value: 'Taiwan',
               label: 'Taiwan',
            }, {
               value: 'Kaohsiung',
               label: 'Kaohsiung',
            }],
            checkList: []
         }
      }
   }
</script>
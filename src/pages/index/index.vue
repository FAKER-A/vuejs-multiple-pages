  <template>
    <div class="app">
        <Header></Header>
        <div style="margin-top:100px">
            <sel-table></sel-table>
        </div>
        
    </div>
</template>

<script>
import Header from '../../components/header'
import selTable from '../../components/sel-table/index'
export default {
    components:{
        Header,
        selTable
    },
    data() {
        return{
            msg:'msg'
        }
    }
}
</script>

<style scoped>
    .app{
        background: #000;
        font-size: 12px;
    }
</style>


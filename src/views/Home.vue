<template>
    <div class="bgView">
        <Layout>
            <Header class="homeHeader">
                <div class="customerNameDiv">
                    客户姓名：
                    <Input prefix="" placeholder="请输入姓名" style="width: 200px" />
                </div>
                <div class="customerTypeDiv">
                    客户类型：
                    <!-- <Input prefix="" placeholder="请输入客户类型" style="width: 200px" /> -->
                    <Select v-model="model1" style="width:200px">
                        <Option v-for="item in data1" :value="item.value" :key="item.value">{{ item.name }}</Option>
                    </Select>
                </div>
                <div class="operateRangeDiv">
                    经营范围：
                    <!-- <Input prefix="" placeholder="请输入经营范围" style="width: 200px" /> -->
                    <Select v-model="model1" style="width:200px">
                        <Option v-for="item in data1" :value="item.value" :key="item.value">{{ item.name }}</Option>
                    </Select>
                </div>
                <div class="creditLevelDiv">
                    信誉等级：
                    <!-- <Input prefix="" placeholder="请输入信誉等级" style="width: 200px" /> -->
                    <Select v-model="model1" style="width:200px">
                        <Option v-for="item in data1" :value="item.value" :key="item.value">{{ item.name }}</Option>
                    </Select>
                </div>
                <div class="customerLevelDiv">
                    客户等级：
                    <!-- <Input prefix="" placeholder="请输入客户等级" style="width: 200px" /> -->
                    <Select v-model="model1" style="width:200px">
                        <Option v-for="item in data1" :value="item.value" :key="item.value">{{ item.name }}</Option>
                    </Select>
                </div>
                <div class="handleDiv">
                    <Button class="searchBtn">
                        查询
                    </Button>
                    <Button class="resetBtn">
                        重置
                    </Button>
                </div>
            </Header>

            <Content class="homeContent">
                <div class="customerMainTitle">客户主表</div>
                <Table class="customerMainTable" height="400" border :columns="columns1" :data="data1"></Table>
                <div class="customerBaseInfoTitle">客户信息表</div>
                <Table class="customerBaseInfoTable" height="200" border :columns="columns1" :data="data1"></Table>
                <div class="customerRelationshipTitle">客户关系表</div>
                <Table class="customerRelationshipTable" height="200" border :columns="columns1" :data="data1"></Table>

            </Content>
        </Layout>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                columns1: [
                    {
                        title: '客户名称',
                        key: 'name'
                    },
                    {
                        title: '办公地址',
                        key: 'age'
                    },
                    {
                        title: '固定电话',
                        key: 'address'
                    },
                    {
                        title: '传真',
                        key: 'address'
                    },
                    {
                        title: '官网',
                        key: 'address'
                    },
                    {
                        title: '客户类型',
                        key: 'address'
                    },
                    {
                        title: '经营范围',
                        key: 'address'
                    },
                    {
                        title: '行业',
                        key: 'address'
                    },
                    {
                        title: '注册资金(万)',
                        key: 'address'
                    },
                    {
                        title: '人员规模',
                        key: 'address'
                    },
                    {
                        title: '信誉等级',
                        key: 'address'
                    },
                    {
                        title: '客户等级',
                        key: 'address'
                    },
                ],
                data1: [
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York',
                        date: '2016-10-03'
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'London',
                        date: '2016-10-01'
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney ',
                        date: '2016-10-02'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York',
                        date: '2016-10-03'
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'London ',
                        date: '2016-10-01'
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney ',
                        date: '2016-10-02'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York ',
                        date: '2016-10-03'
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'London ',
                        date: '2016-10-01'
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney',
                        date: '2016-10-02'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York ',
                        date: '2016-10-03'
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'London ',
                        date: '2016-10-01'
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney',
                        date: '2016-10-02'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },{
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York ',
                        date: '2016-10-03'
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'London ',
                        date: '2016-10-01'
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney',
                        date: '2016-10-02'
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa ',
                        date: '2016-10-04'
                    },
                ],


                columns2: [
                    {
                        title: 'Name',
                        key: 'name',
                        width: 100,
                        fixed: 'left'
                    },
                    {
                        title: 'Age',
                        key: 'age',
                        width: 100
                    },
                    {
                        title: 'Province',
                        key: 'province',
                        width: 100
                    },
                    {
                        title: 'City',
                        key: 'city',
                        width: 100
                    },
                    {
                        title: 'Address',
                        key: 'address',
                        width: 200
                    },
                    {
                        title: 'Postcode',
                        key: 'zip',
                        width: 100
                    },
                    {
                        title: 'Action',
                        key: 'action',
                        fixed: 'right',
                        width: 120,
                        render: (h, params) => {
                            return h('div', [
                                h('Button', {
                                    props: {
                                        type: 'text',
                                        size: 'small'
                                    }
                                }, 'View'),
                                h('Button', {
                                    props: {
                                        type: 'text',
                                        size: 'small'
                                    }
                                }, 'Edit')
                            ]);
                        }
                    }
                ],
                data3: [
                    {
                        name: 'John Brown',
                        age: 18,
                        address: 'New York No. 1 Lake Park',
                        province: 'America',
                        city: 'New York',
                        zip: 100000
                    },
                    {
                        name: 'Jim Green',
                        age: 24,
                        address: 'Washington, D.C. No. 1 Lake Park',
                        province: 'America',
                        city: 'Washington, D.C.',
                        zip: 100000
                    },
                    {
                        name: 'Joe Black',
                        age: 30,
                        address: 'Sydney No. 1 Lake Park',
                        province: 'Australian',
                        city: 'Sydney',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                    {
                        name: 'Jon Snow',
                        age: 26,
                        address: 'Ottawa No. 2 Lake Park',
                        province: 'Canada',
                        city: 'Ottawa',
                        zip: 100000
                    },
                ]
            }
        }
    }
</script>


<style scoped>
    .bgView {
        height: 100%;
        width: 100%;
        min-width: 1280px;
        background-color: lavender;
        overflow: scroll;
        /* padding: 20px 50px 0px 50px; */
    }

    .layout{
        border: 1px solid #d7dde4;
        background: lavender;
        position: relative;
        border-radius: 4px;
        overflow: hidden;
    }

    .layout-logo{
        width: 100px;
        height: 30px;
        background: #5b6270;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
    }

    .layout-nav{
        width: 420px;
        margin: 0 auto;
        margin-right: 20px;
    }
    
    .layout-footer-center{
        text-align: center;
    }


/* 查询条件div */
    .homeHeader {
        display:flex;
        flex-direction: row;
        flex-wrap: wrap;
		/* justify-content:space-between; */
        background-color:white;
        width: 90%;
        height: 90px;
        margin-top: 30px;
        margin-left: 50px;
        border: 1px solid #d7dde4;
    }

    .homeHeader .customerNameDiv {
        float: left;
        margin-top: 10px;
        width: 30%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
    }

    .homeHeader .customerTypeDiv {
        margin-top: 10px;
        width: 30%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
    }

    .operateRangeDiv {
        margin-top: 10px;
        width: 30%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
    }
    
    .creditLevelDiv {
        float: left;
        width: 30%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
    }

    .customerLevelDiv {
        width: 30%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
    }

    .handleDiv {
        width: 27%;
        height: 20px;
        line-height: 20px;
        font-size: 16px;
        justify-content:space-between;
        display:flex;
        flex-direction: row;
    }

    .searchBtn {
        width: 80px;
        height: 30px;
    }

    .resetBtn {
        width: 80px;
        height: 30px;
        /* margin-left: 10px; */
    }

/* 信息展示Div */
    .homeContent {
        margin-top: 10px;
        background-color: rgba(0,0,0,0);
        width: 100%;
        min-height: 100%;
        text-align: center;
    }

    .homeContent .customerMainTitle {
        margin-top: 20px;
        height: 40px;
        line-height: 40px;
        font-size: 15px;
        background-color: white;
        width: 90%;
        margin-left: 50px;
        text-align: left;
        border: 1px solid #d7dde4;
        padding-left: 10px;
    }

    .customerMainTable {
        width: 90%;
        margin-left: 50px;
    }

    .homeContent .customerBaseInfoTitle {
        margin-top: 30px;
        height: 40px;
        line-height: 40px;
        font-size: 15px;
        background-color: white;       
        width: 90%;
        margin-left: 50px;
        text-align: left;
        border: 1px solid #d7dde4;
        padding-left: 10px;

    }

    .customerBaseInfoTable {
        width: 90%;
        margin-left: 50px;
    }

    .homeContent .customerRelationshipTitle {
        margin-top: 30px;
        height: 40px;
        line-height: 40px;
        font-size: 15px;
        background-color: white;
        width: 90%;
        margin-left: 50px;
        text-align: left;
        border: 1px solid #d7dde4;
        padding-left: 10px;

    }

    .customerRelationshipTable {
        width: 90%;
        margin-left: 50px;
    }

</style>
<script>
export default {
    
}

</script>

<template>
    <section id="ratings" class="p-5">
        <table class="table table-borderless">
            <thead>
                <tr>
                    <th scope="col" class="w-75">TEAM</th>
                    <th scope="col">W</th>
                    <th scope="col">D</th>
                    <th scope="col">L</th>
                    <th scope="col">PTS</th>
                </tr>
            </thead>
            <tbody>

                <tr>
                    <th scope="row">
                        <span class="pe-2">1</span>
                        <img src="../assets/img/league-club-1.png" alt="">
                        <span class="ps-2">Istanbul Sports</span> 
                    </th>
                    <td>18</td>
                    <td>2</td>
                    <td>0</td>
                    <td>42</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">2</span>
                        <img src="../assets/img/league-club-2.png" alt="">
                        <span class="ps-2">United Fs Club</span> 
                    </th>
                    <td>14</td>
                    <td>2</td>
                    <td>1</td>
                    <td>35</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">3</span>
                        <img src="../assets/img/league-club-3.png" alt="">
                        <span class="ps-2">Shalcke Club</span> 
                    </th>
                    <td>14</td>
                    <td>2</td>
                    <td>1</td>
                    <td>35</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">4</span>
                        <img src="../assets/img/league-club-4.png" alt="">
                        <span class="ps-2">Inter Club</span> 
                    </th>
                    <td>13</td>
                    <td>2</td>
                    <td>1</td>
                    <td>31</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">5</span>
                        <img src="../assets/img/league-club-5.png" alt="">
                        <span class="ps-2">Madrid Club</span> 
                    </th>
                    <td>12</td>
                    <td>1</td>
                    <td>2</td>
                    <td>30</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">6</span>
                        <img src="../assets/img/league-club-6.png" alt="">
                        <span class="ps-2">Shalcke Club</span> 
                    </th>
                    <td>11</td>
                    <td>0</td>
                    <td>3</td>
                    <td>28</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">7</span>
                        <img src="../assets/img/league-club-7.png" alt="">
                        <span class="ps-2">Arsenal Club</span> 
                    </th>
                    <td>10</td>
                    <td>5</td>
                    <td>0</td>
                    <td>26</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">8</span>
                        <img src="../assets/img/league-club-8.png" alt="">
                        <span class="ps-2">Bayern Club</span> 
                    </th>
                    <td>10</td>
                    <td>2</td>
                    <td>2</td>
                    <td>24</td>
                </tr>

                <tr>
                    <th scope="row">
                        <span class="pe-2">9</span>
                        <img src="../assets/img/league-club-9.png" alt="">
                        <span class="ps-2">Atletico Club</span> 
                    </th>
                    <td>9</td>
                    <td>0</td>
                    <td>4</td>
                    <td>20</td>
                </tr>
            </tbody>

            <tfoot>
                <tr class="text-center">
                    <th scope="col" class="w-100">
                        View Full League Table
                    </th>
                </tr>
            </tfoot>
        </table>
    </section>

</template>


<style lang="scss" scoped>

#ratings {
    min-height: 500px;
    
        table {
            width: 45%;

            th {
                font-weight: normal;

                img {
                    height: 50px;
                }

            }
            
            tr td:last-child{
                font-weight: bold;
            }

            td {
                vertical-align: middle;
            }
        }
}

</style>
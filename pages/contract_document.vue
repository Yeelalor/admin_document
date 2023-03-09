<template>
    <div class="pt-6">
      <div class="pb-4">
        <v-btn color="#358FC4"
          ><span class="white--text">ເພີ່ມຂໍ້ມູນ</span></v-btn
        >
      </div>
      <div style="overflow: scroll; overflow-y: hidden" class="pt-4">
        <table style="border-collapse: collapse; width: 100%">
          <tr style="height: 20px">
            <th style="border: 1px solid #dddddd; text-align: left; padding: 8px">
              ລ.ດ
            </th>
            <th
              style="
                border: 1px solid #dddddd;
                text-align: left;
                padding: 8px;
                height: 30px;
              "
            >
              ເນື້ອໃນຂອງສັນຍາ
            </th>
  
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ເລກທີ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ລົງວັນທີ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ຄູ່ສັນຍາ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ເລກບັນຊີ
            </th>
  
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ມື້ເລີ່ມ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ມື້ສິ້ນສຸດ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ມູນຄ່າສັນຍາ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ສະກຸນເງິນ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ມູນຄ່າຈ່າຍແລ້ວ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ມູນຄ່າຄົງຄ້າງ
            </th>
            <th style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ໝາຍເຫດ
            </th>
          </tr>
          <tr v-for="n in 3" :key="n">
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              1
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ສັນຍາຮັບເໝົາກໍ່ສ້າງ-ຕົບແຕ່ງພາຍນອກອາຄານ ສໍານັກງານໃຫຍ່ ທພລ
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              0266/ທພລ
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              20/01/2022
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ບສ ອາກຄີເນຍ
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              0302000010004185
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              13/01/2022
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              13/01/2025
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              10,264,834,179.79
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              LAK
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              10,264,834,179.79
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              30000
            </td>
            <td style="border: 1px solid #dddddd; text-align: left; padding: 4px">
              ສັນຍາປີຕໍ່ປີ ແຕ່ຂຶ້ນກັບຝ່າຍໄອທີພິຈາະລນາຂໍຕໍ່
            </td>
          </tr>
        </table>
      </div>
    </div>
  </template>
  
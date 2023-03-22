//Method mCari
        System.out.print("Cari : ");
        String cari = sc.next();
        boolean ketemu=false;
        int jumlah=5;
        int idx;
        for (int i = 0; i < jumlah; i++) {
            if(menu_mkn[i].compareToIgnoreCase(cari)==0){
                ketemu=true;
                int idk=i;
                int tmp=idk[i];
                System.out.println(cari+" "+"Ditemukan di index ke-"+idk);
                break;
            }
            
        }
        if(ketemu==false){
            System.out.println("Menu Tidak Ada");
        }

//Method mCari
public static int mCari(String menu_mkn[], int [] harga,){
        Scanner s = new Scanner(System.in);
        System.out.print("Cari : ");
        String cari = s.next();
        String hasil [][]= new String [5][2];
        
        String cariMakan[] = new String [4];
        int cariHarga[]=new int[4];
        int index = 0;
        String status = null;
        System.out.println();
        for (int i = 0; i < menu_mkn.length; i++) {
            if(menu_mkn[i].indexOf(cari)==0){
                hasil[index][0] = menu_mkn[i];
                hasil[index][1] = String.valueOf(harga[i]);
                index++;
                
                System.out.println("No.\tMenu\tHarga");
                status = "ada";
            }  
        }
        if (status!="ada"){
            System.out.println("Menu Tidak Ditemukan");
        }
        int tmp = 0;
        for (int i = 0; i < menu_mkn.length; i++) {
            if (cari==menu_mkn[i]){
                tmp=i;
            }
        }
        return tmp;
    }

//Search Result
System.out.println("==========Search Result==========");
                                System.out.println("No.\tMenu\tHarga");
                                for (int i = 0; i < hasil.length; i++) {
                                    if(hasil[i][0]!=null){
                                        System.out.print((i+1)+"."+hasil[i][0]);
                                        System.out.println("\t"+Integer.parseInt(hasil[i][1]));
                                    }
                                }        

//Laporan Penjualan
for (int i = 0; i < idx_menu; i++) {
                                    if (menu_mkn[i]!=null){
                                        System.out.println((i+1)+"."+"\t"+menu_mkn[i]+"\t"+harga[i]+"\t"+grandTotal);
                                        idx_menu++;
                                        break;
                                    }
                                    
                                }
                                for (int i = 0; i < idx_menu; i++) {
                                    if (laporan_menu[i][0]!=null){
                                        System.out.println((i+1)+"."+"\t"+laporan_menu[idx_own][0]+"\t"+laporan_keuangan [idx_own][0]+"\t"+grandTotal);
                                        idx_own++;
                                        break;
                                    }
                                    
                                }


//Menu Laris
System.out.println("===Daftar Menu Terlaris===");
                                System.out.println("No.\tMenu\tTerjual");
                                String menu_mkn_laris[] = new String [5];
                                menu_mkn_laris=menu_mkn;
                                harga_mkn_laris=porsi;
                                int harga_mkn_laris [] = new int [5];
                                for (int i = 0; i < 5; i++) {
                                    for (int j = 0; j < 4; j++) {
                                        if (harga_mkn_laris[j]>harga[j+1]){
                                            int temp = harga_mkn_laris[j];
                                            harga_mkn_laris[j]=harga_mkn_laris[j+1];
                                            harga_mkn_laris[j+1]=temp;
                                            String temp2 = menu_mkn_laris[j];
                                            menu_mkn_laris[j]=menu_mkn_laris[j+1];
                                            menu_mkn_laris[j+1]=temp2;                           
                                        }
                                    }
                                }
                                for (int i = 0; i < 5; i++) {
                                    System.out.println((i+1)+"."+ "\t" +menu_mkn_laris[i]+ "\t" + harga_mkn_laris[i]);
                                }                              
                                break;

System.out.println("===Daftar Menu Makanan Termahal===");
                        System.out.println("No. \t MENU \t HARGA");
                        String menu_makan2[] = new String [5];
                        menu_makan2=menu_makan;
                        int harga_makan2 [] = new int [5];
                        for (int i = 0; i < 5; i++) {
                            for (int j = 0; j < 4; j++) {
                                if (harga_makan2[j]<harga_makan2[j+1]){
                                    int temp = harga_makan2[j];
                                    harga_makan2[j]=harga_makan2[j+1];
                                    harga_makan2[j+1] = temp;
                                    String temp2=menu_makan2[j];
                                    menu_makan2[j] = menu_makan2[j+1];
                                    menu_makan2[j+1] = temp2;
                                }   
                            }
                        }
                        for (int i = 0; i < 5; i++) {
                            System.out.println((i+1)+"." + menu_makan2[i]+"\t"+harga_makan2[i]);
                        }


menu_mkn[0]="Soto"; harga[0]=10000;
        menu_mkn[1]="Sate"; harga[1]=15000;
        menu_mkn[2]="Bakso"; harga[2]=8000;
        menu_mkn[3]="Rawon"; harga[3]=17000;
        menu_mkn[4]="Gule"; harga[4]=18000;
 

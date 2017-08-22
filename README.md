# ProjectObjectC01
void addIphone(int ptype,int* phone5,int* phone6,int* phone7){

    if(ptype==5){
    
        (*phone5)++;
        
    }else if(ptype==6){
    
        (*phone6)++;
        
    }else if(ptype==7){
    
        (*phone7)++;
        
    }
}
void countIphone(int p1,int p2,int p3,int p4,int p5,int* phone5,int* phone6,int* phone7){

    addIphone(p1,phone5,phone6,phone7);
    
    addIphone(p2,phone5,phone6,phone7);
    
    addIphone(p3,phone5,phone6,phone7);
    
    addIphone(p4,phone5,phone6,phone7);
    
    addIphone(p5,phone5,phone6,phone7);
    
}

int main(int argc, const char * argv[]) {
    
    int iphone5=0,iphone6=0,iphone7=0;
    
    int ns[100]={0};
    int size=sizeof(ns);
    int *p=ns;
    printf("size:%d,psize:%d \n",size,sizeof(p));
    countIphone(5,5,6,7,7,&iphone5,&iphone6,&iphone7);
    printf("iphone5 %d,iphone6 %d,iphone7 %d",iphone5,iphone6,iphone7);
    printf("Hello, World!\n");
    return 0;
    
}

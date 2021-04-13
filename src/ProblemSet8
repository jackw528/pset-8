public class ProblemSet8 {


    public boolean common(int[] a, int[] b) {
        if(a.length == 0 || b.length == 0){
            return false;
        }
        if(a[0] == b[0]){
            return true;
        }else if (a[a.length-1] == b[b.length-1]){
            return true;
        }else{
            return false;
        }
    }

    public int[] middleman(int[] a, int[] b) {

        int[] mmReturn = new int[2];

        if(a == null || b == null || a.length % 2 != 1 || b.length % 2 != 1){
            return null;
        }else {
            mmReturn[0] = a[(a.length-1)/2];
            mmReturn[1] = b[(b.length-1)/2];
            return mmReturn;
        }
    }

    public int[] bigger(int[] a, int[] b) {
    int aSum = 0;
    int bSum = 0;

        if(a == null || b == null){
            return null;
        }else {
            for (int i=0;i < a.length; i++){
                aSum += a[i];
            }
            for (int i=0;i < b.length; i++){
                bSum += b[i];
            }
            if(aSum > bSum){
                return a;
            }else{
                return b;
            }
        }
    }

    public int[] doubleMiddle(int[] a, int[] b) {
        int[] dmReturn = new int[4];

        if(a == null || b == null || a.length % 2 == 1 || b.length % 2 == 1){
            return null;
        }else {
            dmReturn[0] = a[(a.length-1)/2];
            dmReturn[1] = a[(a.length/2)];
            dmReturn[2] = b[(b.length-1)/2];
            dmReturn[3] = b[(b.length/2)];
            return dmReturn;
        }
    }

    public int[] swapMe(int[] a) {
        int temp1;
        int temp2;

        if(a == null){
            return null;
        }
        temp1 = a[0];
        temp2 = a[a.length-1];

        a[0] = temp2;
        a[a.length-1] = temp1;
    return a;
    }

    public int[] threePoint(int[] a) {

        int[] threeArray = new int[3];

            if(a == null || a.length % 2 != 1){
              return null;
            }else {
                threeArray[0] = a[0];
                threeArray[1] = a[(a.length-1)/2];
                threeArray[2] = a[a.length-1];
                return threeArray;
            }
    }

    public int headHoncho(int[] a) {
        boolean intCheck = true;
        int temp;

        for (int i = 0; i < a.length; i++){
            if (a[i] < 0){
                intCheck = false;
            }
        }

        if (a == null || a.length == 0 || intCheck == false){
            return -1;
        }else{

            temp = a[0];
            for (int i = 1; i < a.length; i++){

                if (temp < a[i]){
                    temp = a[i];
                }
            }
            return temp;
        }
    }

    public boolean tippingPoint(int[] a, int threshold) {
        int sum = 0;

        if(a == null){
            return false;
        }else{
            for (int i = 0; i < a.length; i++){

                sum += a[i];

                if (sum > threshold){
                    return true;
                }
            }
        }
        return false;
    }

    public String halfway(int[] a) {
        int left = 0;
        int right = 0;

        if(a == null || a.length == 0 || a.length % 2 != 0){
            return null;
        }else {
            for (int i = 0; i < a.length/2; i++){
                left += a[i];
            }
            for (int i = a.length/2; i < a.length; i++){
                right += a[i];
            }

            if (right > left){
                return "RIGHT";
            }else {
                return "LEFT";
            }
        }
    }

    public int[] sequential(int[] a, int[] b) {

        int[] sequence = new int[3];

        if (a == null || b == null || (a.length + b.length) < 3){
            return null;
        }else if(a.length >= 3) {
            return new int[]{a[0], a[1], a[2]};
        }

        System.arraycopy(a, 0, sequence, 0, a.length);
        System.arraycopy(b,0,sequence,a.length,3-a.length);

        return sequence;
    }
}

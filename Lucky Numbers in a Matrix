import java.util.ArrayList;
import java.util.List;
class Solution {
    public List<Integer> luckyNumbers(int[][] matrix) {
        int N = matrix.length;
        int M = matrix[0].length;
        int[] rowMin = new int[N];
        int[] colMax = new int[M];
        for (int i = 0; i < N; i++) {
            rowMin[i] = Integer.MAX_VALUE;
        }
        for (int i = 0; i < M; i++) {
            colMax[i] = Integer.MIN_VALUE;
        }
        for (int i = 0; i < N; i++) {
            for (int j = 0; j < M; j++) {
                rowMin[i] = Math.min(rowMin[i], matrix[i][j]);
            }
        }
        for (int i = 0; i < M; i++) {
            for (int j = 0; j < N; j++) {
                colMax[i] = Math.max(colMax[i], matrix[j][i]);
            }
        }
        List<Integer> luckyNumbers = new ArrayList<>();
        for (int i = 0; i < N; i++) {
            for (int j = 0; j < M; j++) {
                if (matrix[i][j] == rowMin[i] && matrix[i][j] == colMax[j]) {
                    luckyNumbers.add(matrix[i][j]);
                }
            }
        }
        return luckyNumbers;
    }
    public static void main(String[] args) {
        Solution solution = new Solution();
        int[][] matrix = {
            {3, 7, 8},
            {9, 11, 13},
            {15, 16, 17}
        };
        System.out.println(solution.luckyNumbers(matrix)); 
    }
}

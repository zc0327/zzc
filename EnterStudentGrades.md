# zzc
输入学生成绩，判断等级

		Scanner scan = new Scanner(System.in);
		System.out.println("请输入学生人数：");
		int n = scan.nextInt();
		int[] a = new int[n];
		int max = 0;
		System.out.println("请输入" + n + "个学生成绩：");
		for (int i = 0; i < a.length; i++) {
			a[i] = scan.nextInt();
			if (max < a[i]) {
				max = a[i];
			}
		}
		System.out.println("最高分是：" + max);
		for (int i = 0; i < a.length; i++) {
			String b = "student " + i + " scire is " + a[i] + " grade is ";
			if (max - a[i] <= 10) {
				System.out.println(b + "A");
			} else if (max - a[i] <= 20) {
				System.out.println(b + "B");
			} else if (max - a[i] <= 30) {
				System.out.println(b + "C");
			} else {
				System.out.println(b + "D");
			}
		}

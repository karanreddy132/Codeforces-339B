# Codeforces-339B
#include <bits/stdc++.h>
using namespace std;

int main() {
	long long n, m, curr(1), next, t(0);
	cin >> n >> m;
	for (long long i = 0; i < m; i++) {
		cin >> next;
		if (next >= curr)
			t += next - curr;
		else
			t += n + next - curr;
		curr = next;
	}
	cout << t;
	return 0;
}

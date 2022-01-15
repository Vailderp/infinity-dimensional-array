# infinity-dimensional-array c++ 14
>Examlpe:

````C++
int main()
{
	int D1[] = {
		1, 2,
		3, 4,

		5, 6,
		7, 8
	};

	tu::Data<int, 3>::DataImpl<2, 2, 2> D3 = tu::Data<int, 3>::DataImpl<2, 2, 2>(D1);

    std::cout << *D3.data_ptr[1][1][1] << std::endl;
    std::cout << *D3.data_ptr[1][1][0] << std::endl;
    std::cout << *D3.data_ptr[1][0][1] << std::endl;
    std::cout << *D3.data_ptr[1][0][0] << std::endl;
    std::cout << *D3.data_ptr[0][1][1] << std::endl;
    std::cout << *D3.data_ptr[0][1][0] << std::endl;
    std::cout << *D3.data_ptr[0][0][1] << std::endl;
    std::cout << *D3.data_ptr[0][0][0] << std::endl;
}
````

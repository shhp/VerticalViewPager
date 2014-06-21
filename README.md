VerticalViewPager
=================

The VerticalViewPager is a simple view pager which can be flipped vertically. Unlike the horizontal ViewPager (provided by android-support-v4), you don't have to set a PagerAdapter for the VerticalViewPager. Instead, call VerticalViewPager.setViews(View[]) to supply all page views. You can also set a VerticalViewPager.OnPageChangeListener for the VerticalViewPager. OnPageChangeListener.onPageSelected(int) will be called once a different page is selected.

Usage
=====

Suppose there are three pages to be shown. They are represented by three layout files:

    int[] PAGE_LAYOUTS = new int[]{R.layout.page_one, R.layout.page_two, R.layout.page_three};

Then you can use the VerticalViewPager as follows:

    View[] views = new View[PAGE_LAYOUTS.length];
    for (int i = 0; i < PAGE_LAYOUTS.length; i++) {
        views[i] = LayoutInflater.from(this).inflate(PAGE_LAYOUTS[i], null);
    }
    mViewPager.setViews(views);


Developed By
============

* shhp - <herculeshhp@gmail.com>


License
=======

    Copyright 2014 shhp

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
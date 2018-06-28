# tab切换筛选组件

<div class="dialog-box dialog-label" style="height:2000px;top:120px">
    <div class="dialog-mask"></div>
    <div class="dialog-body">
        <ul class="u-tabs f-clear" data-group="tab">
            <li class="label-title float-l text-c" data-name="年级"><em class="font-weak h1">年级</em></li>
            <li class="label-title float-l text-c  on" data-name="学科"><em class="font-weak h1">学科</em></li>
        </ul>
        <div data-group="tabContent">
            <ul class="m-screen-label mar-r-lgd mar-l-lgd" style="display: none;" data-source="/api/Common/GetGrades"
                data-disable="false" data-disableoriginal="false" data-name="年级">
                <li class="float-l">
                    <ul class="label">
                        <li><a class="u-btn u-btn-lg" data-id="000001">一年级</a></li>
                    </ul>
                </li>
                <li class="float-l">
                    <ul class="label">
                        <li><a class="u-btn u-btn-lg on" data-id="000002">二年级</a></li>
                    </ul>
                </li>
            </ul>
            <ul class="m-screen-label mar-r-lgd mar-l-lgd" style="" data-source="/api/Common/GetCourses"
                data-disable="false" data-disableoriginal="true" data-name="学科">
                <li class="float-l">
                    <ul class="label">
                        <li><a class="u-btn u-btn-lg" data-id="000001">数学</a></li>
                    </ul>
                </li>
                <li class="float-l">
                    <ul class="label">
                        <li><a class="u-btn u-btn-lg" data-id="000002">语文</a></li>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="bars-btn f-clear h1 text-c"><a class="font-weak reset" data-btn="reset">重置</a><a
                class="font-primary" data-btn="ok">确定</a></div>
    </div>
</div>	